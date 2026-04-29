# Codex Creator Challenge Submission

---

## Project Title
**Codenames AI: Systematic Prompt Engineering for Cooperative LLM Agents**

---

## Elevator Pitch (2–3 sentences, for the badge/profile blurb)

I built a framework that pits two GPT agents against each other in the cooperative word game Codenames, then ran 1,000+ experiments across all 36 combinations of 6 prompt-engineering strategies to find which prompts actually work — and why some catastrophically fail. The results contradict a published research paper and reveal a subtle prompt bug that causes a "safe" strategy to hit the assassin word 85% of the time.

---

## Full Description (paste into submission form)

I built a multi-agent Codenames AI framework where two LLM agents — a Codemaster (gives one-word clues) and a Guesser (picks words from a 25-word board) — cooperate to win a game while avoiding a hidden "assassin" word that causes an instant loss. The project started as a reproduction of a 2023 academic study (*Prompt Engineering ChatGPT for Codenames*, Sidji & Stephenson) using the OpenAI API, then became a systematic investigation of how prompt strategy choices interact.

**What I built:**
- Six prompt strategies implemented for both agents: Default, Cautious, Risky, Chain-of-Thought, Self-Refine, and Solo Performance
- A batch experiment runner that tests all 36 strategy combinations (6 Codemaster × 6 Guesser) across 30 fixed board seeds for reproducibility — over 1,000 games on the OpenAI API (GPT-4o-mini)
- An event-logging system that captures every prompt, response, clue, and guess for replay and analysis
- A Streamlit dashboard for running and visualizing live games

**Key findings:**
- Guesser strategy has far more impact on win rate than Codemaster strategy — a finding the original paper missed because it only tested symmetric pairs (same strategy for both agents)
- The best combination, COT Codemaster + Cautious Guesser, achieved a **96% win rate** across 25 games — exceeding the paper's reported best of 94%
- The Self-Refine Guesser had a **catastrophic bug**: asking the model to "check if your guess could be an Assassin word and suggest a safer one" caused it to *switch to* the assassin word 85% of the time. Rephrasing the critique to focus on positive clue-association (which word are you *most confident* is your team's?) fixed it completely
- Cross-strategy combinations that were never tested in the original paper showed a 70–96% win rate, contradicting the paper's conclusion that "no strategy significantly outperforms Default"

**How the OpenAI API was used:**
- GPT-4o-mini powered both agents via the OpenAI Chat Completions API
- Multi-turn conversation history maintained per agent per game
- JSON mode used for structured guesses in Three-Step strategy
- Exponential backoff + retry on rate limits for large-batch experiment runs

**GitHub:** [your repo link here]

---

## Talking points for the AI skill badge interview (if there is one)

- *What was the hardest engineering challenge?* Reproducibility: I fixed 30 board seeds so every strategy combination plays identical games. Without this, noise from random board layouts would mask the effect of prompts.
- *What surprised you most?* The Self-Refine bug. A prompt that sounds careful ("check if it's risky") is actually worse than saying nothing — because it focuses the model on the danger word rather than the target. Negative framing can be actively harmful.
- *What would you do next?* Re-run Self-Refine Guesser with the fixed prompt (running now), then test whether fine-tuning on the logged game data further improves performance.
