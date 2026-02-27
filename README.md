# AlgaSensors Temperature Processing

Temperature Processing is a Spring Boot microservice in the AlgaSensors study project. It focuses on processing temperature events and producing derived signals.

## Responsibilities

- Consume temperature events.
- Apply business rules to detect signals or alerts.
- Persist processed results for reporting or integrations.

## Tech Stack

- Java 21+
- Spring Boot
- Gradle (wrapper included)

## Run Locally

1. Start shared infrastructure from the workspace root:

	docker compose up -d

2. Start this service:

	./gradlew bootRun

## Configuration

- Defaults are in src/main/resources/application.yml.
- Override via environment variables or an external application.yml.

## Related Services

- temperature-monitoring: produces events consumed here.
- device-management: provides device metadata for processing.
