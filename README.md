# POST Event Portal (demo)

A clickable demo of the event-listing workflow for user testing. All events are made up and placed relative to today. Nothing is sent to Notion, Webflow or Event Temple. What a tester types stays in their own browser, and the Reset link clears it.

Live page: https://lovett-group.github.io/post-event-portal-demo/

## Links for embedding in Notion

Use a Notion `/embed` block with one of these links:

| Link | Shows |
|---|---|
| `https://lovett-group.github.io/post-event-portal-demo/` | All three tabs (Events team, Marketing, Client) |
| `…/?role=events` | Events team calendar only |
| `…/?role=marketing` | Marketing calendar only |
| `…/?role=client` | Client asset upload only |

## Client portal (separate page)

`https://lovett-group.github.io/post-event-portal-demo/client.html` is the stand-alone page a client sees from the private link in our email. It shows only their event: confirm details, upload a photo, short description, and optional extras. Uploads are limited to JPG, PNG, WebP (20 MB) and MP4, MOV (200 MB); everything else is refused. In the real version, Brandon's program must repeat these checks on the server and save the files to the event in Notion.

## Editing

Everything is in `index.html`.

- Names in the Owner and "Handled by" dropdowns: the `PEOPLE` list near the top of the script.
- Demo events: the `DEMO` list (days from today, start hour, length, space).
- Example progress: the `EX` list.

Push to `main` and GitHub Pages updates the live page within a minute or two.
