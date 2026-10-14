# Privacy Policy — Full Page Screenshot

Last updated: October 14, 2026

Full Page Screenshot processes screenshots locally in the user's browser. The extension does not operate an account system, analytics SDK, advertising network, remote image-processing service, or screenshot upload endpoint.

## Information handled

When a user explicitly starts a capture, the extension temporarily reads the selected webpage's rendered pixels, layout measurements, scroll position, and page address required to create the requested screenshot and filename.

Temporary screenshot parts, preview data, dimensions, tile coordinates, timing diagnostics, and output format are stored in extension-local browser storage so the capture can be assembled and previewed. Abandoned and expired capture data is removed according to the extension's retention rules.

## How information is used

The information is used only to:

- capture the webpage selected by the user;
- combine captured sections into one continuous image;
- provide a local preview;
- export the result as PNG or PDF; and
- restore the original page state after capture.

## Data sharing and transmission

Screenshot pixels, webpage content, page addresses, and capture metadata are not transmitted to the developer or to third parties. The extension does not sell, transfer, disclose, or use this information for advertising, analytics, profiling, creditworthiness, or any purpose unrelated to its screenshot functionality.

All executable code is included in the extension package. The extension does not download or execute remotely hosted code.

## Data retention and deletion

Capture data remains on the user's device in extension-local storage. Captures are pruned after 24 hours, and no more than the five newest captures are retained. Abandoned image-stitching jobs are pruned after one hour. Users can also remove locally stored extension data by uninstalling the extension or clearing the extension's site data in Chrome.

## Permissions

- `activeTab` provides temporary access only to the tab where the user explicitly starts a capture.
- `scripting` injects the packaged capture script into that active tab to measure and scroll the page.
- `offscreen` provides an extension-owned document for local image decoding, stitching, encoding, and Blob creation.

## Restricted pages

Chrome-managed pages, the Chrome Web Store, and other pages that prohibit extension access cannot be captured. Cross-origin frames are captured as rendered, but the extension cannot independently scroll inaccessible content inside those frames.

## Limited Use

The use of information received from Google APIs will adhere to the Chrome Web Store User Data Policy, including the Limited Use requirements.

## Contact

Privacy and support questions may be submitted at:

https://github.com/WYS012/full_page_screenshot_privacy/issues
