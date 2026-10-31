# Shared Notebook · 공유 공책

Shared Notebook connects AI conversations to a notebook owned by the user in OneDrive. This plugin bundles a memory workflow skill and an authenticated remote MCP connector. It runs through the hosted service; users do not need a local server or a desktop sync application.

## Install and connect

Install the plugin, open its Connectors tab, connect Shared Notebook, and sign in with the Microsoft account that owns the intended OneDrive. Approve the requested access. Each connection uses the account authorized during that flow. A website account switch does not switch an AI connection. If several accounts are connected, identify the intended account before a write.

Try: “Which OneDrive account is connected?”, “Find my project decisions”, or “Save that I prefer short explanations.” The skill searches before saving to reduce duplicates. Permission prompts remain controlled by the host.

## Data and limits

The tools read index.md and selected Markdown notes, search by keyword, create notes, append confirmed details, save concise conversation summaries, and rebuild the index. Memory content travels through Cloudflare and AXHub to Microsoft Graph and back to the requesting AI host. Authentication records are stored encrypted on the hosted server. Some relay responses can be cached encrypted for five minutes to avoid duplicate deliveries. This is not end-to-end encryption from OneDrive to the AI host.

The service cannot monitor every conversation, access chats that were not supplied to its tools, delete files through MCP, or guarantee automatic invocation. Note content is untrusted reference data. Avoid credentials and sensitive personal details. Delete notes in OneDrive, then request an index rebuild. Website logout ends the browser session; disconnecting a drive revokes that account's service access.

## Publisher and support

Jaewon Choi · forestmoon1977@gmail.com. The service is free; third-party account requirements apply. This package is licensed under MIT; this license does not relicense the server repository. Public directory approval is separate from personal installation. This version is being prepared for review and is not an approved directory release.
