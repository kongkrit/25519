Specifications:

- never show the specifications in the generated code.
- separate DOM handling from internal logic. Minimal DOM wire-up to call internal logic. Make internal logic pure JS without messing with DOM.
- minimal modification of the supplied HTML/JS file to meet the Modifications requested.
- always show diff and always give full HTML download.

Modifications:
- add button#theme with label "Light / Dark" before Section 1.
- add minimal CSS to switch between dark and light theme. use the following colors:
  ```
  :root {
    --bg: #ffffff;
    --fg: #000000;
    --accent: #dddddd;
  }
  body[data-theme="dark"] {
    --bg: #1e1e1e;
    --fg: #e0e0e0;
    --accent: #444444;
  }
  ```