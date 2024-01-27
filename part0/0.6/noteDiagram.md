```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: Form Data
    deactivate server

    Note right of browser: 201: The browser does not relead, and it sends no further HTTP requests.
```