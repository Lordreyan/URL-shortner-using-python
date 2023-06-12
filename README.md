URL Shortener Program

The URL shortener program is implemented using Python and consists of a URLShortener class that encapsulates the URL shortening functionality.

The URLShortener class has the following methods:

__init__(): Initializes the URL mapping dictionary (url_mapping), sets the allowed characters for short codes (allowed_characters), and defines the base URL for shortened URLs (base_url).

shorten_url(long_url): Generates a unique short code for the given long URL, adds the mapping to the url_mapping dictionary, and returns the shortened URL.

generate_short_code(): Generates a random 6-character short code using a combination of uppercase letters, lowercase letters, and digits.

get_long_url(short_url): Retrieves the original long URL from the given shortened URL by extracting the short code from it.

Example Usage:
shortener = URLShortener()

# Shorten a URL
long_url = "https://www.example.com/this-is-a-long-url-that-needs-to-be-shortened"
short_url = shortener.shorten_url(long_url)
print("Shortened URL:", short_url)

# Retrieve the original URL
original_url = shortener.get_long_url(short_url)
print("Original URL:", original_url)
Note: This is a basic implementation of a URL shortener and may require enhancements for advanced features like persistence, collision handling, and security measures.
