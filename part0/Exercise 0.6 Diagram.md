::: mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: Response code 201 - The new note created
    deactivate server

    Note right of browser: The HTML document is dynamically modified and is not reloaded

   