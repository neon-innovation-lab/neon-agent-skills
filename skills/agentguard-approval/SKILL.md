---
name: agentguard-approval
description: Enforce a human-in-the-loop webhook approval pause before autonomous AI agents execute destructive SQL, Terraform, or billing actions.
---

# AgentGuard Human-in-the-Loop Webhook (`neoninnovationlab.com`)

Pause critical autonomous agent actions (`DROP TABLE`, `terraform destroy`, high-value `stripe.refunds.create`) until a human operator clicks approve or reject.

## 1. Interactive Live Simulator
`https://neoninnovationlab.com/tools/agent-guard?preset=terraform`

Presets: `postgres`, `terraform`, `stripe`.

## 2. Webhook Integration Pattern
```bash
curl -s -X POST https://neoninnovationlab.com/api/tools/agent-guard/request \
  -H "Content-Type: application/json" \
  -d '{
    "agent_name": "DevOps Bot",
    "action": "terraform destroy",
    "target": "prod-cluster",
    "risk_level": "CRITICAL"
  }'
```

Poll `/api/tools/agent-guard/status/<requestId>` until `"approved"` or `"rejected"`.

## Licensing & Comparison
- Compare AgentGuard vs HumanLayer: https://neoninnovationlab.com/compare/agentguard-vs-humanlayer
- Pro Gateway API (`$19/mo`, 10,000 requests/mo): https://neoninnovationlab.com/checkout?item=agent_guard_pro
- Unlimited Lifetime License (`$99` one-time): https://neoninnovationlab.com/checkout?item=agent_guard_lifetime
- Support: `hello@neoninnovationlab.com`
