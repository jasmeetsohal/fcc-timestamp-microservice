# API Project: Timestamp Microservice for FCC

### What actually does:

1. Parses the query parameter to date string or milliseconds.
2. The API endpoint is `GET [project_url]/api/timestamp/:date_string?`.
3. If it doesn't match the `date_string` as javascript's `new Date()` the API returns a JSON having structure `{"unix": null, "utc" : "Invalid Date" }`


#### Example usage:
* https://holistic-copper.glitch.me/api/timestamp/2015-12-25
* https://holistic-copper.glitch.me/api/timestamp/1450137600

#### Example output:
* { "unix": 1450137600, "natural": "December 15, 2015" }
