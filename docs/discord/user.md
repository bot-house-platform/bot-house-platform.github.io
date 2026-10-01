# User Functions

Functions for retrieving information about Discord users, including IDs, usernames, and display names.

---

## $authorID

Returns the unique Discord snowflake ID of the user who triggered the command.

### Syntax

```

$authorID

```

### Parameters
This function takes no parameters.

### Usage Example

```

$sendMessage[Your user ID is $authorID!]

```

---

## $username

Retrieves the account username of a specified user or the command author.

### Syntax

```

$username[userID]

```

### Parameters
| Parameter | Type | Required | Description |
| :--- | :--- | :--- | :--- |
| `userID` | Number | **No** | The target user's snowflake ID. Defaults to the command author if left blank. |

### Usage Examples

**Retrieve author's username:**

```

$sendMessage[Hello, $username!]

```

**Retrieve specific user's username:**

```

$sendMessage[User details for: $username[123456789012345678]]

```

---

## $displayName

Retrieves the global display name or server nickname for a user.

### Syntax

```

$displayName[userID]

```

### Parameters
| Parameter | Type | Required | Description |
| :--- | :--- | :--- | :--- |
| `userID` | Number | **No** | The target user's snowflake ID. Defaults to the command author if left blank. |

### Usage Examples

**Greeting with display name:**

```

$sendMessage[Welcome back, $displayName!]

```

**In an Embed:**

```

$title[$displayName's Profile]
$description[User ID: $authorID]

```
