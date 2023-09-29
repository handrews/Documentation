---
layout: default
title: Definitions
nav_order: 4
---

# Definitions

- **document**: A local file, network resource, or other distinct entity in a particular format such as JSON or YAML
- **entry document**: The document in an OAD where processing begins, starting with an OpenAPI Object ([3.0](https://spec.openapis.org/oas/v3.0.3#openapi-object), [3.1](https://spec.openapis.org/oas/v3.1.0#openapi-object))
- **link**: Any connection between two parts of an OAD, including but not limited to references
- **OpenAPI Description** (**OAD**): One or more documents written according to a specific version of the OpenAPI Specification, that together describe an API
- **OpenAPI Initiative** (**OAI**): The standards body responsible for the development of the OpenAPI Specification
- **OpenAPI Specification** (**OAS**): The formal requirements for the OpenAPI format, which exists in several versions (e.g. 3.0.3, 3.1.0)
- **reference**: A connection from one location in an OAD to another in which the reference target is identified by a URI; the `"$ref"` and `"operationRef"` keywords implement references in the OAS
- **Uniform Resource Identifier** (**URI**): An identifier for a resource of any kind, which may or may not indicate its location
- **Uniform Resource Locator** (**URL**): A URI intended to be used as a locator for retrieving or otherwise interacting with a resource

## A note on the history of "document", "definition", and "description"

Up through OAS 3.0.3 and 3.1.0, the OAS contained a section titled "OpenAPI Document", with differing definintions depending the OAS version.  The terms "OpenAPI Definition", "OpenAPI Description", and other variations and combinations were also used within the specification and/or the [learn.openapips.org](learn.openapis.org) site.

In September 2023, the OAI Technical Steering Committee (TSC) agreed to standardize on "OpenAPI Description" for the complete logical entity that descrribes an API, and to reserve the term "document" (lower-cased) for its common meaning.  Resolving the debate between "OpenAPI Description" and "OpenAPI Definition" hinged on the observation that while "definition" is appropriate when the API code is generated from the OAD, it is not accurate when an OAD is written for an existing API.  The term "description" is accurate in both cases.

# URIs, URLs, references, servers, and endpoints

The difference between a URI and a URL is the _intended usage_.  While some URI schemes, such as `tag:`, are not suited for use in URLs, even URIs with schemes such as `https:` are not guaranteed to be usable as a URL.

* API servers and endpoints are by definition locations and are therefore URLs
* References use URIs so that they remain the same no matter how your OpenAPI Description's document(s) are stored


## Documents and OpenAPI Descriptions

An OpenAPI Description, or OAD, can be structured as one or more documents.  Those documents are typically stored as local files with `.json` or `.yaml` (or `.yml`) extensions, or as HTTP-accessible network resources of type `application/openapi+json` or `application/openapi+yaml`.

## URIs, URLs, documents, files, and network resources


