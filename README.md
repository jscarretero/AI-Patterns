# AI Engineering Patterns in Python

[Read the book](https://jscarretero.github.io/AI-Patterns)

A practical guide to building applications with language models in Python. It follows a customer support assistant for a fictional online shop, adding one capability at a time and explaining how to test it.

The book covers:

- **Structured outputs and guardrails:** validating model responses and handling unsafe or malformed input.
- **Tool use:** connecting models to functions and APIs, with checks for permissions and repeated actions.
- **RAG:** searching documents, generating answers with citations, and evaluating retrieval.
- **Agents:** building multi-step workflows with budgets, approvals, and recovery after interruptions.
- **Model routing and cascades:** measuring quality, cost, and latency when choosing between models.
- **Batch APIs:** processing offline jobs, handling failures, and resuming interrupted work.

Each part includes Python examples, exercises, and a checkpoint for the shared project. The examples use Pydantic and the Anthropic SDK, with notes on other providers. The book is aimed at engineers who already build services or applications and want to add language models to them.

By Javier Carretero Casado.
