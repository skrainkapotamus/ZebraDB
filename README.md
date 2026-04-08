# ZebraDB
A relational database management system built on data governance.

## Problem Statement
Modern RDBMSs ignore the inherent need of all businesses to manage a production and pre-production instance of their data warehouse and its access privileges. Modern data enterprises can often have enough difficulty achieving data compliance in just their production warehouse alone.

It's normal to use test data in place of production data but this introduces a step of creating test data. It also will always fall short of testing on the actual production dataset. The configuration of an environment shouldn't define the ability to access any given dataset because in reality, a developer could have full, justified access to sensitive data in production and still be unable to query that data because they're in a pre-production environment that isn't aligned with production privileges.

## Proposal
A database managemenet system that is built specifically to be optimized on top of homomorphically encrypted data to enable analytics to be performed with the theoretical possibility of only the end data consumer to actually read the raw data but recognizing the actual scenario where database privileges are able to be factored out of the concept of multiple environments. In other words, if I can access the data to query it in production then I can also access it to test in dev.
