# Exercise 0.6: New note in Single page app diagram

Sequence of events when the user creates a new note using the single-page
app version at `https://studies.cs.helsinki.fi/exampleapp/spa` by writing
into the text field and clicking **Save**.

```mermaid
sequenceDiagram
    participant browser
    participant server

    Note right of browser: User writes a note in the text field and clicks Save

    Note right of browser: The JavaScript event handler prevents the default form submit, adds the new note to the notes list, and re-renders the notes on the page

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    Note right of browser: Sent as JSON in the request body: { "content": "...", "date": "..." }<br/>with header Content-Type: application/json
    activate server
    server-->>browser: 201 Created { "message": "note created" }
    deactivate server

    Note right of browser: No redirect and no page reload — the page was already updated by the JavaScript
```
