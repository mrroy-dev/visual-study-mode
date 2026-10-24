# Visualization rules

## Choose the right format
- Use Mermaid for flowcharts and sequence diagrams when source text is useful.
- Use SVG for crisp, accessible diagrams that need to scale.
- Use Plotly, Observable-style controls, or plain HTML/JavaScript for charts whose controls should update the plot.
- Use tables for exact comparisons and charts for patterns across quantities.
- Prefer a simple, readable figure to a decorative one.

## Interaction requirements
1. Label every control and describe the variable it changes.
2. Make each control update the visualization and any dependent explanation.
3. Provide a reset/default state.
4. Show units, axis labels, legends, and the data source or a clearly marked synthetic-data note.
5. Provide a keyboard-accessible alternative and a short text interpretation.
6. If the environment only supports static Markdown, say so and provide source code or a runnable standalone alternative rather than claiming interactivity.

## Research integrity
- Never create synthetic results that look like results from a paper.
- Mark toy examples and simulated data prominently.
- Do not compare metrics unless their definitions and evaluation conditions are compatible.
