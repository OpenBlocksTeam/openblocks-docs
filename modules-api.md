# Modules API

{% api-method method="get" host="https://api.openblocks.tk" path="/v1/modules" %}
{% api-method-summary %}
Get Modules
{% endapi-method-summary %}

{% api-method-description %}
Get all shared modules.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Authentication" type="string" required=true %}
Auth token, basicly api key.
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
All modules.
{% endapi-method-response-example-description %}

```
{
    "error": 0,
    "modules": [
        {
            "id": "VzSwicwIMH",
            "name": "Module",
            "version": "1.0",
            "description": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tristique consectetur lorem, ut elementum magna accumsan non.",
            "type": "view",
            "author": "TheClashFruit",
            "download": "https://dl.openblocks.tk/VzSwicwIMH.zip",
        }
    ]
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=400 %}
{% api-method-response-example-description %}
Invalid Request
{% endapi-method-response-example-description %}

```
{
    "error": 1,
    "message": "Invalid Auth Token."
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



