# Aura Storage

The idea is to create a graphql on top of mongo db where only diffs of evolving objects are stored.

# Base requirements

This storage stores entities.
Each entity has properties:
* ID
* Body
** Text
** Timestamp
* Revision

Entities evolves with revisions.
Entities are stored in diffs.

## Functions

* Add entity - create an initial revision
* Get entity by ID - retrieve the last revision by reconstructing diffs
* Update entity - write a new revision and store only diff

# Links

https://www.mongodb.com/developer/languages/csharp/interact-graphql-api-dotnet-core-application/
https://dianper.medium.com/building-graphql-api-in-net-core-hotchocolate-mongodb-docker-part-1-d00a20eb0ff0
https://github.com/arackaf/mongo-graphql-starter
https://www.red-gate.com/simple-talk/development/dotnet-development/building-and-consuming-graphql-api-in-asp-net-core-5/