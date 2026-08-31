# Standard-library substitutions

| Normally installed | Used instead | Why |
| --- | --- | --- |
| React / Vue | Browser DOM APIs | The editor renders and updates objects directly in the page. |
| Canvas framework | HTML elements + CSS transforms | Scene objects are draggable, resizable through properties, and stylable without a rendering package. |
| State-management library | Plain JavaScript objects and JSON snapshots | The project state is small, serializable, and inspectable. |
| uuid package | `crypto.randomUUID()` | Gives every scene object an ID using a browser platform API. |
| File-upload library | `<input type="file">` + `FileReader` | Imports image assets and project files with native browser APIs. |
| Download library | `Blob`, `URL.createObjectURL`, and an anchor | Exports a portable project JSON file without a server. |
| Database/backend | `localStorage` | Saves the current project locally in the browser. |
| Animation/timeline library | `requestAnimationFrame` + Web Animations/CSS | Drives playhead playback with platform timing APIs. |

The shipped application is one HTML file and uses no third-party runtime code.
