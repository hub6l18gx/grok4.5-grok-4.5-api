# Grok 4.5 API (grok-4.5 / grok4.5) — llm guide with published pricing

> **input $1.6; output $3.2** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://go.apimart.ai/k-49aff8)** · **[Get an API key](https://go.apimart.ai/k-0aad6f)**

Everything here refers to **grok-4.5** — also written **grok4.5** or **grok 4.5**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `input` | $1.6 |
| `output` | $3.2 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $160 |
| 1,000 | $1,600 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/images/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"grok-4.5","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
