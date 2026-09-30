# API Documentation

Our documentation offers a JSON API endpoint that exposes the list of supported functions, their arguments, descriptions, and metadata. This endpoint can be used to build autocomplete features, syntax highlighters, or custom docs viewers.

---

## Functions List Endpoint

Retrieve a full list of available scripting functions and their parameter signatures.

- **URL:** `/api/discord/cmd.json`
- **Method:** `GET`
- **Response Format:** `application/json`

---

## Response Structure

The endpoint returns an array of function objects structured as follows:

| Field | Type | Description |
| :--- | :--- | :--- |
| `tag` | String | Full function signature (e.g., `$footer[text;footer icon]`). |
| `description` | String | A concise summary of what the function does. |
| `arguments` | Array | List of parameter objects expected by the function. |

### Argument Object Structure

Each object inside the `arguments` array contains:

| Field | Type | Description |
| :--- | :--- | :--- |
| `name` | String | Name of the parameter. |
| `description` | String | Explanation of what to pass for this parameter. |
| `type` | String | Expected data type (`String`, `URL`, `Number`, etc.). |
| `required` | Boolean | Whether the argument is mandatory. |
| `empty` | Boolean | Whether an empty value can be passed. |

---

## Example Response

```json
[
  {
    "tag": "$footer[text;footer icon]",
    "description": "Sets the footer text and optional icon for an embed.",
    "arguments": [
      {
        "name": "text",
        "description": "The footer text.",
        "type": "String",
        "required": true,
        "empty": false
      },
      {
        "name": "footer icon",
        "description": "Direct URL to a footer icon image.",
        "type": "URL",
        "required": false,
        "empty": true
      }
    ]
  }
]
```
