# Exercise 0.4: New note diagram

Sequence of events when the user creates a new note on
`https://studies.cs.helsinki.fi/exampleapp/notes` by writing into the
text field and clicking **Save**.

```mermaid
sequenceDiagram
    participant browser
    participant server

    Note right of browser: User writes a note in the text field and clicks Save

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
    Note right of browser: Form data sent in the request body (note content + date)
    activate server
    server-->>browser: 302 Redirect (Location: /exampleapp/notes)
    deactivate server
    Note right of browser: The server saves the note, then tells the browser to reload the notes page

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/notes
    activate server
    server-->>browser: HTML document
    deactivate server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
    activate server
    server-->>browser: the css file
    deactivate server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.js
    activate server
    server-->>browser: the JavaScript file
    deactivate server

    Note right of browser: The browser starts executing the JavaScript code that fetches the JSON from the server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/data.json
    activate server
    server-->>browser: [{ "content": "...", "date": "2023-1-1" }, ... ] (now includes the new note)
    deactivate server

    Note right of browser: The browser executes the callback function that renders the notes
```

