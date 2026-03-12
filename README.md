# Telecom Event Oracle MCP Server 📡

A premium, high-fidelity Model Context Protocol (MCP) server designed for the 2026 global telecom infrastructure. This oracle provides real-time routing audits, LNP/LRN verification, and proactive congestion pathing for major global events.

## 🏆 2026 Event Readiness
Optimized for high-traffic environments and massive transient network loads:
* **FIFA World Cup 2026:** Specialized routing logic for host city transit.
* **Coachella/Major Festivals:** Proactive pathing for temporary cellular deployments.
* **Carrier Grade:** Built for interoperability between Tier-1 providers and MVNOs.

## 🛠 Features
* `audit_routing`: Analyze phone numbers for Porting (LNP), Location Routing (LRN), and OCN data.
* **Congestion Alerts:** Identifies circular loops and "dead-end" routing paths in real-time.
* **Secure & Monetized:** Powered by xpay.sh for seamless, pay-per-query USDC transactions.

## 🚀 Installation

### For Cursor AI
1. Open **Settings** > **Models** > **MCP**.
2. Click **Add New MCP Server**.
3. Use the following details:
   - **Name:** Telecom Event Oracle
   - **Type:** `sse`
   - **URL:** `https://paywall.xpay.sh/ep_1773326108873_bda3640b81c00051`

### For Claude Desktop / Smithery
Add the following to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "telecom-event-oracle": {
      "command": "npx",
      "args": ["-y", "@xpay/mcp-proxy", "[https://paywall.xpay.sh/ep_1773326108873_bda3640b81c00051](https://paywall.xpay.sh/ep_1773326108873_bda3640b81c00051)"]
    }
  }
}
