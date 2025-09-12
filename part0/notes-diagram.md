# New Note Diagram

```mermaid
SequenceDiagram
    participant browser
    participant server

    browser ->>server: POST https://studies.cs.helsinkl.fi/exampleapp/new_note
    activate server
    server-->>browser: HTML document
    deactivate server

    browser->>server: GET https://studies.cs.helsinkl.fi/exampleapp/notes
    activate server
    server-->>browser: HTML document
    deactivate server

    browser->>server: GET https://studies.cs.helsinkl.fi/exampleapp/main.css
    activate server
    server-->>browser: CSS file
    deactivate server

    browser->>server: GET https://studies.cs.helsinkl.fi/exampleapp/main.js
    activate server
    server-->>browser: JS file
    deactivate server

    browser->>server: GET https://studies.cs.helsinkl.fi/exampleapp/data.json
    activate server
    server-->>browser: JSON file
    deactivate server
```
