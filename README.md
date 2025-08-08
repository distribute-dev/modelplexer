# Modelplexer
> Multiplexer for AI protocols, agents, models, and tools

## Overview
Modelplexer is an operations and orchestration upgrade for your AI applications. By tying together multiple different MCP servers, A2A providers, Identity and auth services, data lookup and retreival systems, and model providers, Modelplexer adds resilience and flexibility to your production apps.

## Project Goals
- Create composable workflows which can be exposed as API endpoints or run on schedules.
- Achieve significant stability and repeatability for Agent/RAG applications without investing large amounts of time.
- Provide plugins for many services such as LangChain scripts, MCP and A2A, vector databases, LLMs, and data sources.
- Move faster in production with code and plugin escape hatches. Assist in evaluating quality.
- Deploy "for real" and successfully serve production traffic.

## Features
Implemented:
- YAML config for expressing Agent/RAG/Chat workflows, routes, and plugins
- Plugins for:
	- Importers: files
	- Vector DBs: DuckDB
	- LLM Services: Ollama
	- Embedders: Ollama
- HTTP server to expose workflows

Planned:
- Pluggable tools with LLM MCP support
- Discover and execute Agents via A2A
- Add intelligent model-informed routing and decision making
- Observability (OpenTelemetry)
- Support for more types of plugins
- More extensive prompt templating

## More information
See [the example config file](./mplex.yaml) to get started. It uses docs from [Kubernetes the Hard Way](https://github.com/kelseyhightower/kubernetes-the-hard-way) (cloned locally) as example data.

Requires Go 1.22+ to build. Default configuration uses Ollama for easy demonstration.

Early experimental phase.

Apache 2.0 Licensed.
Copyright Connor Hicks and contributors, 2025.
