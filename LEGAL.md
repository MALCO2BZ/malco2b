# WorldCam legal and data-use policy

WorldCam is a fork of [Argus](https://github.com/GoSlowPoke168/Argus), released under the MIT License. The original copyright and license notice remain in `LICENSE`.

## What may be reused

- MIT-licensed source code may be modified and redistributed with the copyright and permission notice intact.
- Camera metadata may be imported only from sources that intentionally publish a catalog or API for public viewing.
- Each record should keep its source identifier and, where available, a provenance URL.

## What is excluded

WorldCam does not intentionally discover or publish private devices, credentials, authenticated feeds, proxy-only feeds, or cameras exposed by an apparent network misconfiguration. The ingestion pipeline rejects local/private literal IP targets, credential-bearing URLs, local hostnames, and OpenCCTV records that do not explicitly declare public direct access. A stream URL by itself is not considered permission to display it.

This policy is a product safeguard, not a legal determination. Operators are responsible for respecting each source's terms, robots/API rules, copyright, privacy obligations, and local law. If a source owner asks for removal, remove the record and stop ingesting that source.

## Provenance

`source`, `accessPolicy`, and `provenanceUrl` are carried into generated metadata where a scraper provides them. Duplicate records are collapsed in favor of a native first-party scraper over a discovery bridge.
