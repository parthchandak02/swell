# flux — forex-driven cellular automata

Live exchange rates shape the evolution of a cellular automata colony on a circuit-board grid.

**Visual Style:** Dark — Circuit (digital precision, dot-grid background, green/blue/red palette, right-angle cells)

**Data Source:** Frankfurter API (EUR/USD, EUR/GBP, EUR/JPY exchange rates)

**How it works:**
- Tap any cell to toggle it alive or dead
- Tap empty space to pause or resume the simulation
- EUR/USD, EUR/GBP, and EUR/JPY rates are fetched every 30 seconds from the Frankfurter API
- Rate direction (up/down/flat) tints all alive cells green, red, or pale green
- Volatility between rate updates controls the evolution speed (higher volatility = faster generations)
- The grid initializes randomly and runs Conway's B3/S23 rule with toroidal wrapping

**Live:** https://parthchandak02.github.io/flux/

**Tech:** Native Canvas 2D, single HTML file, zero dependencies.
