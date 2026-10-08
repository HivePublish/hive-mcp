<p><img src="logo.png" width="96" height="96" alt="Hive bee"></p>

# Hive Publish

Official Hive Publish connector package, maintained by Yoav through the `Jebobbes` GitHub account. This repository contains connector configuration and agent guidance. Hive's application source and credentials are not included.

- Product: https://hivepublish.com
- Documentation: https://hivepublish.com/developers
- Privacy: https://hivepublish.com/privacy
- Terms: https://hivepublish.com/terms
- Publisher contact: yoav@hivepublish.com
- Support: support@hivepublish.com
- MCP endpoint: https://hivepublish.com/api/mcp

## Connect from Cursor

Install the Hive plugin, enable its MCP server and sign in to Hive. Choose your workspace and review the requested permissions. Existing connections may need reconnection when the user wishes to grant newly added scopes. A new or empty workspace cannot supply historical social-account metrics.

The Cursor manifest explicitly loads `mcp.json` and `skills/`. The official Hive bee is bundled in `logo.png`. This package does not run local scripts, start builds or store a user's password or provider tokens.

## Current capabilities

Use the live connection's tool list and `read_product_knowledge` to establish what that person can do. Discover additional controls with `list_workspace_operations` and use only its returned operations. Access depends on granted scopes, workspace role, plan, account access and the operation's readiness checks. A package version does not prove every integration, provider account or database prerequisite is ready.

Available controls include publishing and content planning, Honeycomb automations, Hive Bio, analytics and supported Inbox and workspace operations. Card entry, provider sign-in, credential changes and security challenges use the protected browser handoffs returned by Hive.

Writes are marked for confirmation in the AI client. Hive adds exact-action approval when the connection policy requires it, and administration always requires separate Hive approval. The AI cannot approve itself. Private text stays masked by default. A workspace owner or admin must enable both external-AI access and private-body sharing in Inbox privacy settings. Explicit requests for original Inbox text use only the permitted native reveal controls, with the connection's scopes, role checks, confirmation and access audit. Permitted private exports can also contain original information and follow their own scope, access, consent and audit requirements.

## Versions and updates

This connector package is version 1.1.3. The hosted MCP server, plugin package and marketplace listing have independent versions and approval histories. An app deployment updates the common server after it succeeds; it does not automatically approve a marketplace listing, install a new plugin package or expand existing OAuth grants. Refresh the client's tool discovery after a reconnection or permission change.

## Reviewer access

Request dedicated reviewer access through the marketplace's secure review channel or support@hivepublish.com. Credentials are never published in this repository. Reviewer access must be verified before a review is represented as ready: login without extra verification or private-network setup, select the dedicated workspace, complete OAuth, discover permitted tools and execute a permitted read. Use representative test data; do not use customer workspaces or claim fixture data came from a live provider.

## License

MIT. The Hive bee identifies Hive Publish and is not permission to present another product as Hive.
