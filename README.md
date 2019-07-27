# UAA: User Agent Analyser
A php function/library for analysing user agents.

Optimised for Gecko (Firefox), AppleWebKit (Chrome, Safari, Edge) and Trident (Internet Explorer) user agents, but also supports most of the others.

## Usage
```php
include "uaa.php"
$uaa = analyse_user_agent($_SERVER["HTTP_USER_AGENT"]);
$browser_name = $uaa["browser"]["name"];
$browser_version = $uaa["browser"]["version"];
```

## Features
* Detects browser name and version
* Detects operation system (OS) name and version
* Detects device name/identifier if given

## Example return value
```php
array ( "os" => array ( "name" => "Windows", "version" => "10.0" ), "browser" => array ( "name" => "Firefox", "version" => "68.0" ) )
```
