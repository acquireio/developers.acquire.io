---
description: API to add a new sequence
---

# Add

{% api-method method="post" host="https://{{account\_id}}.acquire.io/api/v1/bot/lead" path="" %}
{% api-method-summary %}
Add
{% endapi-method-summary %}

{% api-method-description %}
API to add a new sequence
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
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
    "lead": {
      "title": "Blank Lead",
      "description": "Description",
      "status": "draft",
      "greeting": "active",
      "askFeedback": "disabled",
      "identifier": "blankSequence",
      "identifierCount": 1,
      "isCloned": "no",
      "clonedCount": 0,
      "createdBy": 1,
      "updatedBy": 1,
      "dateCreated": "2021-03-19T04:01:38.050Z",
      "dateUpdated": "2021-03-19T04:01:38.050Z",
      "isImported": "no",
      "id": 139
    }
  }
}

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

## Body\(raw\)

```text
{
  "title": "Blank Lead",
  "description": "Description",
  "status": "draft",
  "greeting": "active",
  "identifier": "blankSequence",
  "askFeedback": "disabled",
  "additionalProp1": {}
}

```
