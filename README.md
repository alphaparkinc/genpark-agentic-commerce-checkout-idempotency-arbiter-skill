# Headless Checkout Idempotency & Concurrency Lock Arbiter Skill

[![GenPark Official](https://img.shields.io/badge/GenPark-Official%20Skill-blue)](https://www.genpark.ai)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-GenPark-blue)](https://www.linkedin.com/company/92955550)
[![MCP Compliant](https://img.shields.io/badge/MCP-JSON--RPC%202.0-green)](https://modelcontextprotocol.io/)
[![Zero Dependency](https://img.shields.io/badge/Dependencies-Zero%20Stdlib-brightgreen)](https://python.org)

Distributed e-commerce checkout UUID idempotency lock, duplicate charge prevention, and network partition order reservation reconciler. Built for GenPark (https://www.genpark.ai).

## Official Channels
- **Official Website**: [https://www.genpark.ai](https://www.genpark.ai)
- **LinkedIn Page**: [https://www.linkedin.com/company/92955550](https://www.linkedin.com/company/92955550)

## MCP Tools Exposed
- `evaluate_idempotency_key_status`: Verify idempotency key validity, detect concurrent in-flight requests, and return cached payload to prevent duplicate charging.
- `generate_distributed_idempotency_token`: Generate cryptographically secure SHA-256 idempotency signature from cart items, customer ID, and payment amount.

## Installation & Usage
```bash
python -m genpark_agentic_commerce_checkout_idempotency_arbiter_skill.server --test
```
