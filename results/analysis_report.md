# Codenames AI Experiment Analysis Report

**Total valid games:** 1736  
**Error entries:** 425

## GEMINI

**Overall:** 256/664 wins (38.6%) | 399 assassin hits

### Strategy Combo Results

| CM Strategy | G Strategy | Games | Wins | Win% | Assassin Hits | Avg Time (s) | Avg Red Found |
|-------------|------------|------:|-----:|-----:|--------------:|-------------:|--------------:|
| COT | Cautious | 15 | 2 | 13.3% | 11 | 232.9 | 4.4 |
| COT | Default | 30 | 4 | 13.3% | 26 | 262.2 | 4.1 |
| COT | Self Refine | 21 | 1 | 4.8% | 19 | 247.7 | 3.6 |
| COT | Solo Performance | 30 | 5 | 16.7% | 25 | 205.1 | 4.2 |
| Cautious | COT | 28 | 12 | 42.9% | 16 | 51.7 | 6.0 |
| Cautious | Cautious | 28 | 10 | 35.7% | 18 | 90.7 | 5.7 |
| Cautious | Default | 26 | 13 | 50.0% | 13 | 24.6 | 5.8 |
| Cautious | Risky | 30 | 7 | 23.3% | 23 | 507.9 | 5.5 |
| Cautious | Self Refine | 30 | 16 | 53.3% | 14 | 422.0 | 6.2 |
| Cautious | Solo Performance | 29 | 12 | 41.4% | 17 | 34.1 | 5.6 |
| Default | COT | 28 | 15 | 53.6% | 13 | 35.4 | 6.1 |
| Default | Cautious | 29 | 17 | 58.6% | 12 | 17.1 | 6.4 |
| Default | Default | 30 | 12 | 40.0% | 18 | 15.2 | 6.1 |
| Default | Risky | 29 | 13 | 44.8% | 16 | 11.2 | 5.7 |
| Default | Self Refine | 30 | 6 | 20.0% | 20 | 25.8 | 5.2 |
| Default | Solo Performance | 28 | 11 | 39.3% | 17 | 250.1 | 5.1 |
| Risky | COT | 30 | 17 | 56.7% | 13 | 55.2 | 6.0 |
| Risky | Cautious | 30 | 19 | 63.3% | 11 | 27.8 | 6.7 |
| Risky | Default | 30 | 12 | 40.0% | 18 | 19.2 | 5.7 |
| Risky | Risky | 30 | 16 | 53.3% | 14 | 18.6 | 6.4 |
| Risky | Self Refine | 30 | 4 | 13.3% | 24 | 33.2 | 5.2 |
| Risky | Solo Performance | 30 | 9 | 30.0% | 21 | 20.5 | 5.5 |
| Self Refine | Cautious | 13 | 9 | 69.2% | 4 | 73.7 | 7.2 |
| Self Refine | Default | 30 | 14 | 46.7% | 16 | 71.0 | 6.2 |

### Codemaster Marginal Performance

| CM Strategy | Games | Wins | Win% | Assassin Hits |
|-------------|------:|-----:|-----:|--------------:|
| Default | 174 | 74 | 42.5% | 96 |
| Cautious | 171 | 70 | 40.9% | 101 |
| Risky | 180 | 77 | 42.8% | 101 |
| COT | 96 | 12 | 12.5% | 81 |
| Self Refine | 43 | 23 | 53.5% | 20 |

### Guesser Marginal Performance

| G Strategy | Games | Wins | Win% | Assassin Hits |
|------------|------:|-----:|-----:|--------------:|
| Default | 146 | 55 | 37.7% | 91 |
| Cautious | 115 | 57 | 49.6% | 56 |
| Risky | 89 | 36 | 40.4% | 53 |
| COT | 86 | 44 | 51.2% | 42 |
| Self Refine | 111 | 27 | 24.3% | 77 |
| Solo Performance | 117 | 37 | 31.6% | 80 |

## OPENAI

**Overall:** 604/1072 wins (56.3%) | 448 assassin hits

### Strategy Combo Results

| CM Strategy | G Strategy | Games | Wins | Win% | Assassin Hits | Avg Time (s) | Avg Red Found |
|-------------|------------|------:|-----:|-----:|--------------:|-------------:|--------------:|
| COT | COT | 30 | 21 | 70.0% | 9 | 67.4 | 6.7 |
| COT | Cautious | 25 | 24 | 96.0% | 1 | 71.5 | 7.9 |
| COT | Default | 30 | 18 | 60.0% | 11 | 140.6 | 6.6 |
| COT | Risky | 30 | 20 | 66.7% | 10 | 52.3 | 7.1 |
| COT | Self Refine | 30 | 3 | 10.0% | 25 | 69.2 | 4.6 |
| COT | Solo Performance | 30 | 22 | 73.3% | 8 | 44.6 | 7.4 |
| Cautious | COT | 30 | 18 | 60.0% | 12 | 294.7 | 5.9 |
| Cautious | Cautious | 30 | 25 | 83.3% | 5 | 25.2 | 7.2 |
| Cautious | Default | 30 | 19 | 63.3% | 11 | 29.6 | 6.9 |
| Cautious | Risky | 30 | 17 | 56.7% | 13 | 21.7 | 6.3 |
| Cautious | Self Refine | 30 | 1 | 3.3% | 25 | 35.5 | 4.7 |
| Cautious | Solo Performance | 30 | 24 | 80.0% | 6 | 28.6 | 7.1 |
| Default | COT | 30 | 18 | 60.0% | 12 | 493.3 | 6.5 |
| Default | Cautious | 30 | 20 | 66.7% | 10 | 1309.5 | 7.2 |
| Default | Default | 28 | 18 | 64.3% | 10 | 19.8 | 7.0 |
| Default | Risky | 30 | 17 | 56.7% | 13 | 16.0 | 6.6 |
| Default | Self Refine | 30 | 2 | 6.7% | 27 | 25.7 | 4.4 |
| Default | Solo Performance | 30 | 19 | 63.3% | 11 | 16.1 | 7.0 |
| Default | Three Step | 30 | 17 | 56.7% | 13 | 74.3 | 5.8 |
| Risky | COT | 30 | 16 | 53.3% | 14 | 69.0 | 6.0 |
| Risky | Cautious | 29 | 21 | 72.4% | 8 | 19.5 | 7.0 |
| Risky | Default | 30 | 18 | 60.0% | 12 | 19.4 | 6.6 |
| Risky | Risky | 30 | 19 | 63.3% | 10 | 15.6 | 6.8 |
| Risky | Self Refine | 30 | 2 | 6.7% | 25 | 40.7 | 4.0 |
| Risky | Solo Performance | 30 | 17 | 56.7% | 12 | 16.2 | 6.6 |
| Self Refine | COT | 30 | 18 | 60.0% | 12 | 1651.3 | 6.7 |
| Self Refine | Cautious | 30 | 27 | 90.0% | 3 | 397.7 | 7.6 |
| Self Refine | Default | 30 | 20 | 66.7% | 10 | 71.2 | 7.1 |
| Self Refine | Risky | 30 | 20 | 66.7% | 10 | 102.8 | 7.0 |
| Self Refine | Self Refine | 30 | 2 | 6.7% | 27 | 158.3 | 4.0 |
| Self Refine | Solo Performance | 30 | 24 | 80.0% | 6 | 92.2 | 7.2 |
| Solo Performance | COT | 30 | 20 | 66.7% | 9 | 93.9 | 6.3 |
| Solo Performance | Cautious | 30 | 26 | 86.7% | 4 | 70.2 | 7.3 |
| Solo Performance | Default | 30 | 16 | 53.3% | 14 | 57.8 | 6.2 |
| Solo Performance | Risky | 29 | 13 | 44.8% | 16 | 44.7 | 6.3 |
| Solo Performance | Self Refine | 30 | 1 | 3.3% | 24 | 109.4 | 4.4 |
| Solo Performance | Solo Performance | 1 | 1 | 100.0% | 0 | 58.9 | 8.0 |

### Codemaster Marginal Performance

| CM Strategy | Games | Wins | Win% | Assassin Hits |
|-------------|------:|-----:|-----:|--------------:|
| Default | 208 | 111 | 53.4% | 96 |
| Cautious | 180 | 104 | 57.8% | 72 |
| Risky | 179 | 93 | 52.0% | 81 |
| COT | 175 | 108 | 61.7% | 64 |
| Self Refine | 180 | 111 | 61.7% | 68 |
| Solo Performance | 150 | 77 | 51.3% | 67 |

### Guesser Marginal Performance

| G Strategy | Games | Wins | Win% | Assassin Hits |
|------------|------:|-----:|-----:|--------------:|
| Default | 178 | 109 | 61.2% | 68 |
| Cautious | 174 | 143 | 82.2% | 31 |
| Risky | 179 | 106 | 59.2% | 72 |
| COT | 180 | 111 | 61.7% | 68 |
| Self Refine | 180 | 11 | 6.1% | 153 |
| Solo Performance | 151 | 107 | 70.9% | 43 |
