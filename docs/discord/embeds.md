# Embed Functions

Embed functions allow you to customize the layout and visual presentation of rich Discord embeds.

---

## `$title`

Sets the title of the current embed.

### Syntax
```bdscript
$title[text]
```

### Parameters
| Parameter | Type | Required | Description |
| :--- | :--- | :--- | :--- |
| `text` | String | Yes | The header title for the embed. |

### Example
```bdscript
$title[Server Rules]
```

---

## `$description`

Sets the main description text for the embed.

### Syntax
```bdscript
$description[text]
```

### Parameters
| Parameter | Type | Required | Description |
| :--- | :--- | :--- | :--- |
| `text` | String | Yes | The main content body of the embed. |

### Example
```bdscript
$description[Please be respectful to everyone in the server.]
```

---

## `$footer`

Adds a footer banner at the bottom of the embed, with an optional icon.

### Syntax
```bdscript
$footer[text;footer icon]
```

### Parameters
| Parameter | Type | Required | Description |
| :--- | :--- | :--- | :--- |
| `text` | String | Yes | Text shown at the bottom of the embed. |
| `footer icon` | URL | No | Direct URL to an image for the footer icon. |

### Example
```bdscript
$footer[Page 1 of 5;https://example.com/footer-icon.png]
```

---

## `$thumbnail`

Displays a small image in the top-right corner of the embed.

### Syntax
```bdscript
$thumbnail[image url]
```

### Parameters
| Parameter | Type | Required | Description |
| :--- | :--- | :--- | :--- |
| `image url` | URL | Yes | A valid image URL (`http://` or `https://`). |

### Example
```bdscript
$thumbnail[https://example.com/logo.png]
```

---

## `$image`

Displays a large, full-width image inside the main body of the embed.

### Syntax
```bdscript
$image[image url]
```

### Parameters
| Parameter | Type | Required | Description |
| :--- | :--- | :--- | :--- |
| `image url` | URL | Yes | A valid image URL (`http://` or `https://`). |

### Example
```bdscript
$image[https://example.com/banner.png]
```