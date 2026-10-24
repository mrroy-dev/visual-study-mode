# Visual Study Mode

**By MrRoy** · An open learning skill for ChatGPT-style assistants and Claude-style skill workflows.

Visual Study Mode helps people learn technical topics and research papers through step-by-step explanations, source-grounded analysis, editable visualization guidance, practice questions, and study notes.

## Features

- Step-by-step concept teaching with intuition, formal definitions, and worked examples
- Research-paper breakdowns: problem, method, results, assumptions, limitations, and reproducibility
- Visual-first learning with editable chart/diagram guidance and honest static fallbacks
- Model/method comparison with clear criteria and uncertainty
- Practice questions and adaptive review
- Export-friendly notes and runnable examples
- Source-integrity rules to avoid fabricated citations or paper results

## Repository contents

- `skills/visual-study-mode/SKILL.md` — main portable skill instructions
- `skills/visual-study-mode/references/visualization-rules.md` — visualization and evidence rules
- `assets/visual-study-mode-icon.png` — square brand icon
- `assets/visual-study-mode-banner.png` — promotional banner/mockup

## Use with Claude Code

This repository is a Claude plugin marketplace containing the `visual-study-mode` plugin in `plugins/visual-study-mode/`.

In Claude's Plugins settings, choose **Add marketplace**, enter `mrroy-dev/visual-study-mode` (or this repository's Git URL), and sync. The repository must be pushed to GitHub with the marketplace and plugin manifests before Claude can sync it.

```sh
claude plugin marketplace add mrroy-dev/visual-study-mode
claude plugin install visual-study-mode@visual-study-mode-marketplace
```

To install from a local checkout, run `claude plugin marketplace add .` from the repository root, then install the plugin with the command above.

The plugin exposes the skill as `/visual-study-mode:visual-study-mode`.

## Use as a standalone Claude skill

1. Download or clone this repository.
2. Open the `skills/visual-study-mode/` folder.
3. Follow the platform's current instructions for importing a custom skill; if a ZIP upload is supported, zip that folder's contents and upload it.
4. Test it with a concept explanation and a research-paper PDF.

## Use with ChatGPT

The skill files are portable instructions, not a guarantee of a universally installable ChatGPT plugin. ChatGPT plugin availability and import flows depend on the current product and account. You can use the `SKILL.md` as project instructions in a supported custom GPT/project/workflow, or install the separately published private plugin if you have access to it.

## Use with other assistants

Copy the `SKILL.md` instructions into the assistant's supported custom-instructions, project, or skill mechanism. Keep the reference file alongside it if the platform supports reference files.

## Important capability note

The skill provides a workflow and implementation guidance. It does **not** itself host a web app or automatically create live interactive charts in every chat interface. For true interactive controls, the host must support interactive UI or the assistant must provide a runnable HTML/JavaScript/SVG implementation.

## Contributing

Issues and pull requests are welcome. Please:
- Include a clear reproduction prompt for behavior issues.
- Keep examples source-grounded and mark synthetic data.
- Do not add private data, copyrighted full-text papers, secrets, tokens, or API keys.
- Test the skill with both a concept lesson and a paper-analysis prompt.
- Explain accessibility and static-fallback behavior for new visualizations.

See [CONTRIBUTING.md](CONTRIBUTING.md).

## Roadmap

- More worked visualization examples
- Paper-analysis checklist and reproducibility rubric
- Accessibility review for diagrams and charts
- Multilingual teaching examples
- Automated skill regression test prompts

## License

MIT. See [LICENSE](LICENSE).
