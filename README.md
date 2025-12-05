# AI Model Timeline

An interactive visualization tracking the release dates and benchmark performance of major AI/LLM models from 2022 to present.

[Live Demo](https://models.indulge.digital) | [GitHub](https://github.com/patthewebrat/model-releases-timeline)

## Features

- **Timeline view**: Visual timeline showing model releases by quarter with organization and model names
- **Benchmark chart**: Dual-axis chart displaying MMLU and HLE (Humanity's Last Exam) scores over time
- **Comments**: Notable events and context for significant releases
- **Dynamic data**: Reads from CSV file for easy updates

## Data

The timeline data is stored in `models_benchmarks.csv` with the following columns:

| Column | Description |
|--------|-------------|
| Quarter | Release quarter (e.g., Q1 2023) |
| Model | Model name |
| Organisation | Company/organization |
| Date | Release date (MM/DD/YY) |
| MMLU | MMLU benchmark score (%) |
| HLE | Humanity's Last Exam score (%) |
| Notes | Additional notes about the model |
| Comments | Notable events displayed on timeline |

## Usage

Serve the files via a local web server (required for CSV loading due to browser security restrictions).

```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve

# Using PHP
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

## Models Tracked

Includes major releases from:
- OpenAI (GPT series, o1, Sora)
- Anthropic (Claude series)
- Google (Gemini series, PaLM)
- Meta (LLaMA series)
- xAI (Grok series)
- Alibaba (Qwen series)
- DeepSeek
- Microsoft (Bing Chat)

## Built by

[Indulge Digital](https://indulge.digital)
