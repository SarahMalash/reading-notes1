# read 11
1. package.json will hold our Node application information and the dependencies we need
2. server.js: will hold our Express server setup, configuration. We'll define our routes to our pages here.

## Looping Over Data
To loop over our data, we will use (forEach)

# Using the API
Every request your application sends to the  API needs to identify your application to Google. 
*There are two ways to identify your application:* using:
1. an OAuth 2.0 token  and/or 
2. using the application's API key.
 Here's how to determine which of those options to use:
 1. If the request requires authorization then the application must provide an OAuth 2.0 token with the request. *The application may also provide the API key, but it doesn't have to.*
2. If the request doesn't require authorization then the application must provide either the API key or an OAuth 2.0 token, or both—whatever option is most convenient for you.

### Authorizing requests with OAuth 2.0
1. When you create your application, you register it using the Google API Console. Google then provides information you'll need later, such as a client ID and a client secret.
2. Activate the Books API in the Google API Console. (If the API isn't listed in the API Console, then skip this step.)
3. When your application needs access to user data, it asks Google for a particular scope of access.
4. Google displays a consent screen to the user, asking them to authorize your application to request some of their data.
5. If the user approves, then Google gives your application a short-lived access token.
6. Your application requests user data, attaching the access token to the request.
7. If Google determines that your request and the token are valid, it returns the requested data.

### Acquiring and using an API key:
*Requests to the Books API for public data must be accompanied by an identifier, which can be an API key or an access token.*

*To acquire an API key:*

1. Open the Credentials page from this url (https://console.developers.google.com/projectselector2/apis/credentials?pli=1&supportedpurview=project) in the API Console.
2. This API supports two types of credentials. Create whichever credentials are appropriate for your project:
*OAuth 2.0: Whenever your application requests private user data, it must send an OAuth 2.0 token along with the request. Your application first sends a client ID and, possibly, a client secret to obtain a token. You can generate OAuth 2.0 credentials for web applications, service accounts, or installed applications.*

*API keys: A request that does not provide an OAuth 2.0 token must send an API key. The key identifies your project and provides API access, quota, and reports.*

The API supports several types of restrictions on API keys. If the API key that you need doesn't already exist, then create an API key in the Console by clicking Create credentials > API key. You can restrict the key before using it in production by clicking Restrict key and selecting one of the Restrictions.

### Google Books IDs
Volume IDs - Unique strings given to each volume that Google Books knows about. An example of a volume ID is _LettPDhwR0C. You can use the API to get the volume ID by making a request that returns a Volume resource; you can find the volume ID in its id field.
Bookshelf IDs - Numeric values given to a bookshelf in a user's library. Google provides some pre-defined shelves for every user with the following IDs:
Favorites: 0
Purchased: 1
To Read: 2
Reading Now: 3
Have Read: 4
Reviewed: 5
Recently Viewed: 6
My eBooks: 7


## IDs on Google Books site
1. Volume ID:
When viewing a particular volume on the site, you can find the volume ID in the id URL parameter.

2. Bookshelf ID
When viewing a particular bookshelf on the site, you can find the bookshelf ID in the as_coll URL parameter.

3. User ID:
When viewing your library on the site, you can find the user ID in the uid URL parameter.

### Working with volumes
This request has a single required parameter:

q - Search for volumes that contain this text string. There are special keywords you can specify in the search terms to search in particular fields, such as:
intitle: Returns results where the text following this keyword is found in the title.
inauthor: Returns results where the text following this keyword is found in the author.
inpublisher: Returns results where the text following this keyword is found in the publisher.
subject: Returns results where the text following this keyword is listed in the category list of the volume.
isbn: Returns results where the text following this keyword is the ISBN number.
lccn: Returns results where the text following this keyword is the Library of Congress Control Number.
oclc: Returns results where the text following this keyword is the Online Computer Library Center number.





