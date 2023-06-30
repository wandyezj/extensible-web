# API

- Definition
- Discovery
- Implementation

## Contract

The framework should enforce the API contract.

- Version available.
- Allowable Argument Types
- Returned Data Types
- Types of errors

## Types of APIs

- Single Calls
- Batched Calls
- Events

## API Definition

There needs to be an easy way to design, implement, and consume APIs.

Ideally APIs are defined and then implementation stubs are generated to be filled in. Everything else should be automatically handled by the extension framework.

### Generated

- Stubs
- Intellisense for consuming extension
- Documentation

## API Helpers

`isApiSupported` - check if an API is supported by the host website. Important when there are multiple versions of the host website. Multiple versions can occur when websites are instances of particular frameworks.

## Design

An extension needs to know when the extension client is ready to be used.

## Batched Calls

When there is overhead to making API calls, it is useful to batch calls together.

It's convenient if this framework can be generated from the existing async APIs.