# Episode Query

This directory contains a GraphQL query to fetch a specific episode by ID from the Rick and Morty API.

## Files

- `episode-page-1.graphql`: Query to fetch episode with ID 1
- `characters-page-1-output.json`: Expected output for characters page 1
- `characters-page-2.graphql`: Query to fetch characters page 2
- `characters-page-2-output.json`: Expected output for characters page 2
- `characters-page-3.graphql`: Query to fetch characters page 3
- `characters-page-3-output.json`: Expected output for characters page 3
- `characters-page-4.graphql`: Query to fetch characters page 4
- `characters-page-4-output.json`: Expected output for characters page 4

## Query Structure

```graphql
query GetEpisode {
  episode(id: 1) {
    id
    name
    air_date
    episode
  }
}
```
