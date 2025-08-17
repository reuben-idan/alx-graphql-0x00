# Character Queries

This directory contains GraphQL queries to fetch character information from the Rick and Morty API.

## Individual Character Queries

- `character-id-1.graphql`: Query to fetch character with ID 1
- `character-id-1-output.json`: Expected output for character ID 1
- `character-id-2.graphql`: Query to fetch character with ID 2
- `character-id-2-output.json`: Expected output for character ID 2
- `character-id-3.graphql`: Query to fetch character with ID 3
- `character-id-3-output.json`: Expected output for character ID 3
- `character-id-4.graphql`: Query to fetch character with ID 4
- `character-id-4-output.json`: Expected output for character ID 4

## Paginated Character Queries

- `characters-page-1.graphql`: Query to fetch page 1 of characters
- `characters-page-1-output.json`: Expected output for page 1
- `characters-page-2.graphql`: Query to fetch page 2 of characters
- `characters-page-2-output.json`: Expected output for page 2
- `characters-page-3.graphql`: Query to fetch page 3 of characters
- `characters-page-3-output.json`: Expected output for page 3
- `characters-page-4.graphql`: Query to fetch page 4 of characters
- `characters-page-4-output.json`: Expected output for page 4

## Query Structure

### Single Character Query
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

### Paginated Characters Query
```graphql
query GetCharacters($page: Int) {
  characters(page: $page) {
    info {
      count
      pages
      next
      prev
    }
    results {
      id
      name
      status
      image
    }
  }
}
```
