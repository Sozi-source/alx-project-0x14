## API Overview
For this project i will be using a movie database API endpoint to fetch favourites movies. 

The API documentation has the following sections:
### Getting Started
This section gives a brief description of what the API does.

### Authentication
This section requires the user to login before accessing the api key.

### My request
It stores a history of all the API request made by a client.

### HTTP METHODS
The API documentation details two HTTP methods i.e GET and POST.


## API VERSION
The API uses V3 which is the default version.

## Available Endpoints
https://api.themoviedb.org/3/account/{account_id}/favorite/tv: This is an endpoint for favourite TV.
https://api.themoviedb.org/3/account/{account_id}/favorite/movies: Endpont for favourite Movies
https://api.themoviedb.org/3/account/{account_id}/rated/movies: endpoint for rated movies

## Authentication
API allows auth by allowing special information sent in the HTTP request header section to prove you have the permission to access the API.

## Error Handling
400: bad request
401: unauthorized
403: forbidden
404: not found
500: internal server error
503: service unavailable

## Usage Limits and Best Practices
1. Common Usage Limitations
Rate Limits → API restrict number of reqest.
Data Size Limits → limit size of the response
Endpoint Restrictions → Some routes may require higher-tier accounts or special permissions.

2. Best Practices
**Batch Requests → Combine multiple requests into one when possible.
**Cache Responses → Save results locally to avoid hitting the server repeatedly for the same data.
**Use Pagination → If an API returns large lists, fetch them in chunks rather than all at once.
**Handle Rate Limits Gracefully → If you get an HTTP 429 Too Many Requests, pause and retry after the given Retry-After time.
**Secure Your Credentials → Never hardcode tokens in public code; store them in environment variables.
**Minimize Unnecessary Calls → Only call the API when the data is actually needed.
**Respect API Terms → Stay within the provider’s guidelines to avoid getting blocked.