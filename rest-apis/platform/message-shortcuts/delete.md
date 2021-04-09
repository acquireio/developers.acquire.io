---
description: API to delete the shortcuts
---

# Delete

{% api-method method="delete" host="https://{{account\_id}}.acquire.io/api/v1/crm/message-shortcut?id={{shortcutId}}" path="" %}
{% api-method-summary %}
Delete
{% endapi-method-summary %}

{% api-method-description %}
Delete a message shortcut. The **shortcutId** must be passed in to the endpoint as a query parameter. **Warning**: This action cannot be undone. 
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="shortcutId" type="integer" required=true %}
Array of shortcuts ids to be deleted
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
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
    "deleted": 1
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}


