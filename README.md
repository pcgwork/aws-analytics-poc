# AWS Analytics POC

End-to-end data pipeline demonstration using AWS cloud and modern backend stack.

## Scope
Track user events from a web app and make them queryable in minutes.

## Flow
React (TypeScript) → Quarkus (Kotlin) API → Kafka → S3 → Glue → Athena

## Components
- **frontend/**: React app that captures and sends events
- **api/**: Quarkus service to validate and publish events to Kafka
- **kafka/**: Kafka + Connect setup for S3 sink
- **glue/**: Glue ETL and crawlers
- **infra/**: Deployment scripts (ECS, S3, IAM)
- **docs/**: Diagrams and notes

## Tech Stack
React, TypeScript, Kotlin, Quarkus, Kafka, AWS S3, Glue, Athena

## Goal
Event in UI → stored → transformed → queried via Athena within 5 minutes
