# Messaging Functions

Functions used to dispatch and control messages within a channel.

---

## `$sendMessage`

Sends a text message along with any created embed objects to the current channel.

### Syntax
```bdscript
$sendMessage[text]
```

### Parameters
| Parameter | Type | Required | Description |
| :--- | :--- | :--- | :--- |
| `text` | String | Yes | Plain text content to send alongside the embed response. |

### Example
```bdscript
$title[Announcement]
$description[Maintenance starting in 10 minutes!]
$sendMessage[Attention @everyone!]
```