<p align="center">
  <img src="assets/founder-signal.svg" alt="Buptrain — product-minded engineering" width="100%" />
</p>

# Building useful software with clear boundaries

I build focused developer and consumer tools that turn messy, real-world workflows into understandable software. I care about the details that make a product trustworthy: a legible workflow, deliberate permissions, local-first defaults where they fit, and honest constraints.

For founders, potential technical cofounders, and investors, this profile is a compact record of how I think about product and execution: start with a specific job, make the system inspectable, and ship the smallest useful surface.

## Selected work

| Product | The problem | What is in the repository |
| --- | --- | --- |
| [BillSplitter](https://github.com/buptrain/fi-expense-extension) | Shared mobile plans create a recurring coordination problem: reading carrier PDFs, allocating costs, and settling up. | A Chrome side-panel extension that parses supported Google Fi and T-Mobile statements locally, produces a reviewable per-person split, and opens an optional pre-filled payment request. |
| [StreamLoader](https://github.com/buptrain/streamloader) | People sometimes need an offline copy of media they are authorized to keep, without turning the workflow into a general-purpose scraper. | A Manifest V3 Chrome extension that detects direct MP4 streams in the current tab, keeps the results per-tab, and provides copy, open, and download actions with practical filename handling. |

## How I build

- **Product first.** I frame features around the user's decision or workflow, not a technology list.
- **Local when appropriate.** BillSplitter parses statements in the browser; neither project requires an account or a service for its core path.
- **Permission-aware systems.** StreamLoader's repository explains its browser permissions and limits itself to direct, authorized MP4 workflows.
- **Constraints are part of the product.** Carrier statement formats can change; segmented streams and DRM are out of scope. Clear failure modes are more useful than implied magic.

## Technical signal

The current work is intentionally small and concrete:

- Chrome Manifest V3, side panels, service workers, content scripts, and local extension storage
- Client-side PDF text extraction with carrier-specific parsing and allocation logic
- Per-tab state, network-event observation, declarative request rules, and resilient download handling
- Product documentation that treats privacy, permissions, and limitations as first-class design decisions

## Open to the right conversation

I am interested in early product work where technical judgment and user experience need to evolve together—especially practical tools that reduce coordination, improve clarity, or respect the user's data and attention.

If you are a founder, potential technical collaborator, or investor who values that kind of execution, the project READMEs above are the best place to start.
