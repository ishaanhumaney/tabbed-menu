# Tabbed Menu

A simple, fast, and structured restaurant menu UI that switches categories instantly without a single line of JavaScript. 

By abusing hidden radio inputs and the CSS general sibling combinator (`~`), this project implements clean UI tab switching directly in the browser's style engine. It is built entirely with semantic HTML5 and vanilla CSS3.

## Value Proposition & Architecture

Most modern web apps bundle megabytes of JavaScript just to toggle visibility states on a page. This project uses the built-in state management of HTML forms (`:checked`) to manage UI states. 

* **Zero JavaScript:** No dependencies, no framework overhead, and zero runtime script execution.
* **Instant State Transitions:** Category filtering happens natively inside the browser's layout engine.
* **Semantic Structure:** Leverages native `<input type="radio">` and `<label>` relations to remain structured and predictable.

## Tech Stack Breakdown

* **HTML5:** Structuring tabular views using standard form controls for accessible keyboard and click targets.
* **CSS3:** Handling state transitions using `:checked` combined with the `~` sibling selector. No styling hacks—just layout rules.

## Project Structure

```text
├── index.html     # Page structure, menu data, and state-holding radio buttons
└── style.css      # Component layout, structural resets, and visibility toggles
```

## Quick Start (Browser-Only Setup)
You don't need a terminal, Git, or Node.js to spin this up. You can preview and edit it completely in your browser.

1. **Launch with GitHub Codespaces:** Click the Code button on this repository, select the Codespaces tab, and click Create codespace on main.

2. **Preview:** Once inside the web editor, open index.html, click the Go Live button at the bottom right, or use a browser preview extension to view it live.

Alternatively, you can click on the index.html file right here on GitHub, copy the code, paste it into a local text file, and double-click it to run it instantly in any browser.

## Roadmap
[ ] Add smooth opacity fade-in transitions for category switching.

[ ] Implement CSS Grid to turn the single-column menu into a multi-column responsive grid on larger displays.

[ ] Inject ARIA attributes to enhance screen reader accessibility for hidden radio setups.
