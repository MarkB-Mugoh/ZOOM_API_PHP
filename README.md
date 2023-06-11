
# ZOOM_API_PHP

The "zoom-api-php" repository on GitHub is a collection of PHP code examples and libraries that demonstrate how to integrate the Zoom API into a PHP application. The repository provides a set of pre-built classes that wrap the Zoom API endpoints, making it easy to interact with the API from PHP code.

The repository includes examples of how to use the Zoom API to perform tasks such as creating and managing meetings, managing users and webinars, and retrieving reports. Additionally, the repository includes a set of scripts that demonstrate how to authenticate with the Zoom API using JSON Web Tokens (JWTs).

This repository is a valuable resource for PHP developers who want to integrate the Zoom API into their applications. By using the pre-built classes and examples provided in the repository, developers can quickly get up and running with the Zoom API, saving them time and effort in the integration process.







## How to run the project

Clone the directory into your server path 
```bash
/opt/lampp/htdocs/zoomFolder
```
Define the API key and the secret key.
remember to change the email too
```bash
define('API_KEY','');
define('API_SECRET','');
define('EMAIL_ID','example@gmail.com');
```
Create a Zoom account: at https://zoom.us/signup.

Create a JWT App under developer settings: Next, create a JWT App in the Zoom App Marketplace. This app will provide you with an API key and API secret that you can use to authenticate your requests to the Zoom API.

# How to update the library
To update the php-jwt package in PHP, you can follow these steps:

Check the current version of the php-jwt package that you have installed by running the following command in your terminal:

```bash
composer show firebase/php-jwt
```
If there is a new version available, you can update the package by running the following command in your terminal:

```bash
composer update firebase/php-jwt
```
This command will update the php-jwt package to the latest version.

After updating the package, make sure to update any references to the php-jwt package in your PHP code to use the new version.

For example, if you previously used the following code to generate a JWT token:

```bash
use Firebase\JWT\JWT;

$token = JWT::encode($payload, $secret);
```
You should update it to:

```
use Firebase\JWT\JWT;

$token = JWT::encode($payload, $secret, 'HS256');
```
This is because the default signing algorithm for JWT tokens changed from HS256 to RS256 in version 4.0.0 of the php-jwt package.

That's it! Your php-jwt package is now updated to the latest version.

Remember to cutomise the code to fit your project requirements.

The JWT app type will be depreceated june 1, 2023 by zoom. You should consider to create server to sever Oauth or an Oauth app to replace the functionality of a JWT app in your zoom account




