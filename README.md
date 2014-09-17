=== PassportPCI API PHP Wrapper ===

You can sign up for a PassportPCI account at [passportpci.com](https://passportpci.com)

== Requirements ==

PHP 5.2 or later

== Setup ==

Obtain the latest version of the PassportPCI PHP bindings with:

git clone https://github.com/passportpci/passportpci-php
To use the bindings, add the following to your PHP script:

require_once("/path/to/passportpci-php/lib/PassportPCI.class.php");

== Getting Started ==
	
Simple usage looks like:

PassportPCI::setClientId("9K7xN98Nny");
PassportPCI::setClientSecret("9e9Q66evykXR8D63");

$resp = PassportPCI::getCardToken(array(
		"appkey" => "123456789", //this is your api public key
		"cardnumber" => "4111111111111111",
		"expmonth" => "2016",
		"expyear" => "11")
);

print_r($resp);

== Documentation ==

Please see [PassportPCI API docs](https://api.passportpci.com/docs/) for up-to-date documentation.

== Tests ==