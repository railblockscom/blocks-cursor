# MCP Servers

Model Context Protocol (MCP) servers extend Cursor's agent capabilities with external tools and data sources.

## Setup

1. Copy `mcp.json` to `~/.cursor/mcp.json`
2. Replace placeholder tokens with your actual credentials
3. Restart Cursor to load the new MCP servers

---

## Available MCPs

### Context7

**Purpose:** Retrieve up-to-date documentation and code examples for any library or framework.

**Use when:**
- Building integrations with third-party services
- Working with frameworks or libraries (React, Next.js, Stripe, etc.)
- Need current API documentation or usage examples

**Setup:** No authentication required.

**Docs:** https://context7.com

---

### Supabase

**Purpose:** Manage Supabase projects, run SQL, deploy edge functions, and more.

**Use when:**
- Working with Supabase databases
- Deploying edge functions
- Managing migrations and branches

**Setup:** Requires a Supabase access token.
1. Go to https://supabase.com/dashboard/account/tokens
2. Generate a new access token
3. Replace `<YOUR_SUPABASE_ACCESS_TOKEN>` in mcp.json

**Docs:** https://supabase.com/docs/guides/getting-started/mcp

---

### Convex

**Purpose:** Interact with Convex backend - run queries, manage data, view logs.

**Use when:**
- Working with Convex databases
- Running functions or queries
- Debugging backend issues

**Setup:** Run `npx convex login` first to authenticate.

**Docs:** https://docs.convex.dev/

---

### Greptile

**Purpose:** AI-powered code search and review across repositories.

**Use when:**
- Need to understand large codebases
- Want AI-assisted code reviews
- Searching for patterns across repos

**Setup:** Requires a Greptile API key.
1. Sign up at https://greptile.com
2. Get your API key from the dashboard
3. Replace `<YOUR_GREPTILE_API_KEY>` in mcp.json

**Docs:** https://docs.greptile.com

---

### Axiom

**Purpose:** Query logs and observability data from Axiom.

**Use when:**
- Debugging production issues
- Analyzing logs and traces
- Monitoring application performance

**Setup:** Authentication handled via Axiom's OAuth flow in Cursor.

**Docs:** https://axiom.co/docs

---

### Dub Documentation

**Purpose:** Search Dub's documentation for link management APIs.

**Use when:**
- Building link shortening features
- Integrating with Dub's API
- Working on analytics for links

**Setup:** No authentication required.

**Docs:** https://dub.co/docs

---

### PostHog

**Purpose:** Query analytics and feature flag data from PostHog.

**Use when:**
- Working with product analytics
- Managing feature flags
- Debugging user behavior issues

**Setup:** Authentication handled via PostHog's OAuth flow in Cursor.

**Docs:** https://posthog.com/docs
