REST Guidelines
===

![Riot Emergence Logo](./riot-emergence-logo.png)

REST uidelines for Riot Emergence projects

---
- [Collections in Plural](#collections-in-plural)
- [Use Natural Identifiers Always That Is Possible](#use-natural-identifiers-always-that-is-possible)
- [Where Natural Identifiers Cannot Be Used, Use The P-R-G Pattern](#where-natural-identifiers-cannot-be-used-use-the-p-r-g-pattern)
- [Composite Identifiers In Aggregated Resources URLs](#composite-identifiers-in-aggregated-resources-urls)
---

# REST Is Not only a Language For Web Services, It Is a Language For The Web

# Use The Browsers Behavior As Base For Your Web Service Behavior

The Web Browsers are the de facto tool when using the Web. They are created for exceptional people and institutions, that created the specs that Web are made. Studying their behavior and imitating they on your Web Service are the best way to create a testable and standard-compliant Application.

# English as Resource Language

The english language is the most used language in the world and is the "de fato" language for computing and internet. Most of the tecnologies used today in Internet and development were developed in english and use APIs in english. Most standardization institutions publish their specs in english (ISO, IETF, ITU-T, etc...)

# Collections in Plural

Always use collections in plural so it will be easy to identify a resource as a collection.

Eg: Collection of Persons
http://example.com/persons

Eg: Collection of Teams
http://example.com/teams

# Use Natural Identifiers Always That Is Possible

The use of natural identifiers instead of surrogate keys makes easier to remember an URL and makes the use of HTTP PUT method in both creation and update reducing code to implement both funcionalities. 
The PUT method has the advantage of being idempotent.

# Where Natural Identifiers Cannot Be used, Use The P-R-G Pattern

The Post-Redirect-Get Pattern is a pattern.

# When using HTTP PUT, Diferentiate The Result Code Based on Insertion or Creation.

When using PUT, return HTTP Status Code 201 if the resource was created and 200 

# Composite Identifiers in Aggregated Resources URLs

Eg: A Person: 
http://example.com/persons/john-smith

Eg: A Team: 
http://example.com/teams/the-falcons

Eg: An Aggregation: 
http://example.com/teams-formations/the-falcons/john-smith
