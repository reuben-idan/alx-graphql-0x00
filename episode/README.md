# Episode Queries

This directory contains GraphQL queries to fetch episode information from the Rick and Morty API.

## Files

- `episode-1.graphql`: Query to fetch episode with ID 1
- `episode-1-output.json`: Expected output for episode ID 1
- `episode-2.graphql`: Query to fetch episode with ID 2
- `episode-2-output.json`: Expected output for episode ID 2
- `episode-3.graphql`: Query to fetch episode with ID 3
- `episode-3-output.json`: Expected output for episode ID 3
- `episode-4.graphql`: Query to fetch episode with ID 4
- `episode-4-output.json`: Expected output for episode ID 4

## Query Structure

Each query follows this structure:

```graphql
query GetEpisode($id: ID!) {
  episode(id: $id) {
    id
    name
    air_date
    episode
  }
}
```
