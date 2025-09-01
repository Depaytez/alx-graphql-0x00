# GraphQL Practice with Ricky and Murty API 
This task involves writing GraphQL queries to fetch details of specific characters from the Rick and Morty GraphQL API (https://rickandmortyapi.com/graphql). The queries retrieve data for characters with IDs 1, 2, 3, and 4, including the fields id, name, status, species, type, and gender.

## Purpose
The goal is to practice constructing precise GraphQL queries to request specific data, using the character(id: ID!) field. This demonstrates how to avoid over-fetching data and use arguments to filter results by ID.

## Files
1. episode-page-1.graphql
2. characters-page-1-output.json
3. characters-page-2.graphql
4. characters-page-2-output.json
5. characters-page-3.graphql
6. characters-page-3-output.json
7. characters-page-4.graphql
8. characters-page-4-output.json

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