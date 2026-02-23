## What is Summa?

Summa is a **general-purpose open-source ledger** designed to record any type of asset transaction. This can include financial transactions, loyalty and gaming points transactions, logistic transactions, and more.

The modern transactional world demands systems that can handle complex movements of assets while maintaining **high levels of consistency, availability, and instantaneity**. These attributes are notoriously challenging to achieve to any degree of simultaneity with traditional tools.

## How Summa Achieves These Attributes?

<!-- Talk about TigerBeetle and importante advantages that it brings that make Summa fast -->

- Strict Serializability:
- ACID-compliant:
- Single-threaded: (say something about shard too)
- Batching:
- High Availability:
- Extreme Engineering:
- Storage Fault Tolerance:

### So, Why Not Use TigerBeetle Directly?

<!-- talk also that tigerbeetle is a low level database, a trusted component -->
<!-- after all, introduces Identity and Access Management -->

## Identity and Access Management

Summa supports OAuth2 by default to allow own IAM providers. And for access 

## Data Schema

Summa is built on simple, yet powerful primitives:
- **Asset**: any unit of value (USD, EUR, Loyalty Points, Tokens...).
- **Account**: a container for a specific asset balance (Checking, Savings, Wallets, Liabilities, Revenues, Expenses...).
- **Balance**: the current amount held in an account for a specific asset.
- **Transaction**: an atomic financial event composed of multiple postings.
- **Operation**: the granular unit of movement (debit/credit) that must always balance to zero.

## Getting Started

### Running with Docker

The fastest way to get Summa up in a development environment and running is via Docker Compose:

```shell
# Clone the repository
git clone git@github.com:gabrielribeirof/summa.git
cd summa

# Set environment variables for local environment
make set-env

# Start all services
make up
```

## Acknowledgements & Inspirations

Summa is a practical exercise in high-performance software engineering, heavily inspired by:

[Midaz by LerianStudio](https://github.com/LerianStudio/midaz) for the powerful reference in multi-asset accounting.

[TigerBeetle](https://github.com/tigerbeetle/tigerbeetle) for setting the bar on performance and safety.