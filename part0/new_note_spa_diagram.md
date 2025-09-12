# New Note Diagram
```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server GET https://studies.cs.helsinki.fi/exampleapp/spa
    server activated
    server-->>browser: HTML document
    server deactivated

    browser->>server GET https://studies.cs.helsinki.fi/exampleapp/main.css
    server activated
    server-->>browser: CSS document
    server deactivated

    browser->>server GET https://studies.cs.helsinki.fi/exampleapp/spa.js
    server activated
    server-->>browser: Javascript file
    server deactivated

    browser->>server GET https://studies.cs.helsinki.fi/exampleapp/data.json
    server activated
    server-->>browser: JSON file is given to browser and parsed
    server deactivated

    browser->>server GET https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    server activated
    server-->>browser: JSON file is parsed to JS file so notes SPA updates with new note added
```
