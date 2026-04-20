# SuperOPSAgent

> Intelligent Q&A and O&M System based on Spring Boot + AI Agent

## Project Introduction

Enterprise-level intelligent business agent system, containing two core modules:

### 1. RAG Intelligent Q&A
Integrates Milvus vector database and Alibaba Cloud DashScope to provide intelligent Q&A capabilities based on Retrieval-Augmented Generation, supporting multi-turn conversations and streaming output.

### 2. AIOps Intelligent Operations
AI Agent-based automated operations system, adopting Planner-Executor-Replanner architecture, achieving alarm analysis, log querying, intelligent diagnosis and report generation.

## Core Features

- ✅ **RAG Q&A**: Vector retrieval + Multi-turn conversation + Streaming output
- ✅ **AIOps Operations**: Intelligent diagnosis + Multi-Agent collaboration + Automatic reporting
- ✅ **Tool Integration**: Document retrieval, alert querying, log analysis, time tools
- ✅ **Session Management**: Context maintenance, history management, automatic cleanup
- ✅ **Web Interface**: Provides test interface and RESTful API


## Tech Stack

| Technology | Version | Description |
|------------|---------|-------------|
| Java | 17 | Development Language |
| Spring Boot | 3.2.0 | Application Framework |
| Spring AI | - | AI Agent Framework |
| DashScope | 2.17.0 | Alibaba Cloud AI Services |
| Milvus | 2.6.10 | Vector Database |

## Core Modules

```
SuperBizAgent/
├── src/main/java/org/example/
│   ├── controller/
│   │   └── ChatController.java        # Unified Interface Controller
│   ├── service/
│   │   ├── ChatService.java           # Conversation Service
│   │   ├── AiOpsService.java          # AIOps Service
│   │   ├── RagService.java            # RAG Service
│   │   └── Vector*.java               # Vector Services
│   ├── agent/tool/                    # Agent Tools
│   │   ├── DateTimeTools.java         # Time Tools
│   │   ├── InternalDocsTools.java     # Document Retrieval
│   │   ├── QueryMetricsTools.java     # Alert Querying
│   │   └── QueryLogsTools.java        # Log Querying
│   └── config/                        # Configuration Classes
├── src/main/resources/
│   ├── static/                        # Web Interface
│   └── application.yml                # Application Configuration
└── aiops-docs/                        # O&M Documentation Library
```