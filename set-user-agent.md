We have conventions for setting user agents in projects that make API calls. This helps us to understand which projects are useful to developers.

The User-Agent header should follow this convention:

`nexmo-<language>/<client_version> <language>/<language_version> <app_name>/<app_version>`

Client libraries set the language and nexmo client version, and should accept a parameter for a demo app to add the final segment, so we end up with something like

`nexmo-php/1.2.3 php/7.3.1 my-app/12.3.4`

