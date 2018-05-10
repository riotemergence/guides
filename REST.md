REST Guidelines
===

![Riot Emergence Logo](./riot-emergence-logo.png)

REST uidelines for Riot Emergence projects

---
- [Collections in Plural](#collections-in-plural)
- [Use Natural Identifiers Always That Is Possible](#use-natural-identifiers-always-that-is-possible)
- [Where Natural Identifiers Cannot Be Used, Use The P-R-G Pattern](##where-natural-identifiers-cannot-be-used-use-the-p-r-g-pattern)
- [Composite Identifiers In Aggregated Resources URLs](#composite-identifiers-in-aggregated-resources-urls)
---

# Collections in Plural

Eg: Collection of Persons
http://example.com/persons

Eg: Collection of Teams
http://example.com/teams

# Use Natural Identifiers Always That Is Possible

The use of natural identifiers instead of surrogate keys is easier to remember and makes the use of HTTP PUT method when using 
Natural identifiers implies
The PUT method has the advantage of being idempotent.

# Where Natural Identifiers Cannot Be used, Use The P-R-G Pattern

The Post-Redirect-Get Pattern

# Composite Keys in Aggregated Resources URLs

Eg: A Person: 
http://example.com/persons/john-smith

Eg: A Team: 
http://example.com/teams/the-falcons

Eg: An Aggregation: 
http://example.com/teams-formations/the-falcons/john-smith
