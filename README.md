# GraphQL Practice with Ricky and Murty API 
This task involves writing GraphQL queries to fetch details of specific characters from the Rick and Morty GraphQL API (https://rickandmortyapi.com/graphql). The queries retrieve data for characters with IDs 1, 2, 3, and 4, including the fields id, name, status, species, type, and gender.

## Purpose
The goal is to practice constructing precise GraphQL queries to request specific data, using the character(id: ID!) field. This demonstrates how to avoid over-fetching data and use arguments to filter results by ID.

## Files
1. character-id-1.graphql: Query for character ID 1.
2. character-id-1-output.json: JSON output for character ID 1.
3. character-id-2.graphql: Query for character ID 2.
4. character-id-2-output.json: JSON output for character ID 2.
5. character-id-3.graphql: Query for character ID 3.
6. character-id-3-output.json: JSON output for character ID 3.
7. character-id-4.graphql: Query for character ID 4.
8. character-id-4-output.json: JSON output for character ID 4.

## How It Was Done
* Each query was written and tested using the GraphiQL interface at https://rickandmortyapi.com/graphql.

* The queries specify the character(id: ID!) field with IDs 1, 2, 3, and 4, requesting id, name, status, species, type, and gender.

* The JSON outputs from GraphiQL were saved as corresponding .json files.

Example Query
```graphql
query GetCharacter {
  character(id: 1) {
    id
    name
    status
    species
    type
    gender
  }
}
```

Example Output
```json
{
  "data": {
    "character": {
      "id": "1",
      "name": "Rick Sanchez",
      "status": "Alive",
      "species": "Human",
      "type": "",
      "gender": "Male"
    }
  }
}
```