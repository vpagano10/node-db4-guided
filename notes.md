# Data Modeling Notes

## Requirements

A client has hired you to build an API for managing `zoos` and the `animals` kept at each `zoo`. The API will be used for `zoos` in the _United States of America_, no need to worry about addresses in other countries.

For the `zoos` the client wants to record:

- name.
- address.

For the `animals` the client wants to record:

- name.
- species.
- list of all the zoos where they have resided.

Determine the database tables necessary to track this information.
Label any relationships between table.

# A good data model (opinion)

- captures ALL the data needed by the system
- captures ONLY the data needed by the system
- reflects reality (from the point of view of the system)
- is felxible (can grow or shrink with the needs of the system)
- guarantee data integrity (without sacrificing too much performance)
- is driven by the way we access the data

# Components

- entities (resources): nouns --> tables
- properties (column, fields, attributes) --> columns
- relationships --> foreign keys

# Workflow
- entities (resources): nouns --> tables
- properties (column, fields, attributes) --> columns
- relationships --> foreign keys

# Relationships

- one to one: rare
- one to many: most common
- many to many: smoke and mirros

# Mantras

- Every table must have a primary key
- Work on 2 or 3 entities at a time (narrow your focus)
- one to many: relationship requires a 'Foreign Key'
- The 'Foreign Key' goes on the many side of the relationship
- many to many: requires a 3rd table
- the 3rd table can have other columns (that are not the foreign keys)
