## Selected work

| Product | The problem | What is in the repository |
| --- | --- | --- |
| [EmuXR](https://github.com/buptrain/emuxr) | Classic game rendering is usually fixed to a flat screen. EmuXR explores whether rendering-layer information can create a playful, optional spatial presentation without hiding the original view. | A clean-room Android XR proof of concept: an instrumented mGBA rendering path connects through an engine-independent C ABI to a Unity 6 URP/OpenXR frontend. It includes original and experimental 2.5D views, controller input, save/load, and documented Galaxy XR validation. |
| [BillSplitter](https://github.com/buptrain/fi-expense-extension) | Shared mobile plans create a recurring coordination problem: reading carrier PDFs, allocating costs, and settling up. | A Chrome side-panel extension that parses supported Google Fi and T-Mobile statements locally, produces a reviewable per-person split, and opens an optional pre-filled payment request. |
| [StreamLoader](https://github.com/buptrain/streamloader) | People sometimes need an offline copy of media they are authorized to keep, without turning the workflow into a general-purpose scraper. | A Manifest V3 Chrome extension that detects direct MP4 streams in the current tab, keeps the results per-tab, and provides copy, open, and download actions with practical filename handling. |

## How I build

- **Product first.** I frame features around the user's decision or workflow, not a technology list.
- **Local when appropriate.** BillSplitter parses statements in the browser; neither project requires an account or a service for its core path.
- **Permission-aware systems.** StreamLoader's repository explains its browser permissions and limits itself to direct, authorized MP4 workflows.
- **Constraints are part of the product.** Carrier statement formats can change; segmented streams and DRM are out of scope. Clear failure modes are more useful than implied magic.
- **Prototype with a compatibility fallback.** EmuXR keeps the original resolved screen available while making 2.5D spatial presentation an explicit experiment, not a promise about every game.
