Project: Tiny URL Shortener
1. Requirements:

Functional: Shorten URL, Redirect URL.
Non-Functional: Low Latency, High Availability.
2. API Design:

POST /shorten -> returns short URL.
GET /{code} -> redirects to long URL.
3. Database:

Key-Value pair (Code | Long URL).
Use SQL or Redis.
4. Algorithm:

Base62 Encoding (Convert unique ID to string).
