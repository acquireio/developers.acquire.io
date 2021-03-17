# Delete note

{% api-method method="delete" host="https://{{account\_id}}.acquire.io/api/v1/crm/note/{noteId}" path="" %}
{% api-method-summary %}
Delete a note
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="noteId" type="string" required=false %}
ID of the note 
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=false %}
Bearer {{api\_key}}
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
  "data": {
    "success": true,
    "message": "Note has been deleted successfully."
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}
