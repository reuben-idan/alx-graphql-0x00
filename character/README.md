# Character Queries

This directory contains GraphQL queries to fetch character information from the Rick and Morty API.

## Files

- `character-id-1.graphql`: Query to fetch character with ID 1
- `character-id-1-output.json`: Expected output for character ID 1
- `character-id-2.graphql`: Query to fetch character with ID 2
- `character-id-2-output.json`: Expected output for character ID 2
- `character-id-3.graphql`: Query to fetch character with ID 3
- `character-id-3-output.json`: Expected output for character ID 3
- `character-id-4.graphql`: Query to fetch character with ID 4
- `character-id-4-output.json`: Expected output for character ID 4

## Query Structure

Each query follows this structure:

```graphql
query GetCharacter($id: ID!) {
  character(id: $id) {
    id
    name
    status
    species
    type
    gender
  }
}
```
