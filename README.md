# SE333 Assignment 6: UI Testing with Playwright

## Project Overview: 

Automated UI testing for DePaul University bookstore using Playwright. 
This project includes manual UI test automation and AI-assisted test generation 
with GitHub Actions.

![Playwright UI Tests](https://github.com/sptl01/SE333-Assignment-6/actions/workflows/playwright.yml/badge.svg)


## Reflection – Manual vs AI‑Assisted UI Testing

### Manual UI Testing (`playwrightTraditional`)
*Wrote the test step‑by‑step in Java + Playwright.*

- **Pros** – Full control over selectors, explicit waits, and edge‑case handling.
- **Cons** – Time‑consuming, fragile selectors required many fallbacks (`input[id*='search']`, `button:has‑text('Add to Cart')`).

### AI‑Assisted UI Testing (`playwrightLLM`)
*Generated with Playwright MCP using the prompt*

- **Pros** – Time saving to generate a runnable JUnit test. Took 10 minutes to get complate running code.
- **Cons** – Uses simpler `text=` selectors, missed a few assertions, required minor manual tweaks for reliability.
