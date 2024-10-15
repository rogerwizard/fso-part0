# New note in single page app diagram
```mermaid
sequenceDiagram
    participant browser
    participant server

    Note right of browser: The Browser creates creates the note object and renders the new note/sends it to the server
    
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa with note content/creation date
    activate server
    server-->>browser: 301 Created
    deactivate server
```
