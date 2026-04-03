# ZebraDB
A database built on data governance. Leverages zero-knowledge theory to create a single dataset safe for both production and development / pre-production environments.

## Problem Statement
Modern RDBMSs ignore the inherent need of all businesses to manage a production and pre-production instance of their data warehouse. It's normal to use test data in place of production data but this introduces a step of creating test data. It also will always fall short of testing on the actual production dataset. The configuration of an environment shouldn't define the ability to access any given dataset.

## Proposal
Zero-knowledge theory is an active area of research because of its potential applicability to solve real-world problems. It's generally applied to an entire dataset, but if it were applied at a more granular level such as to every cell of data in a database file, it would allow a user that knows in their mind what data they are querying and expecting to interact with the same dataset from SQL while keeping the raw, potentially sensitive data masked.
