# 🤝 Partnership Management

Welcome to the official repository for our partner list! This repository manages the data for all our partner communities, which is displayed by our Discord bots and on our official website.

## 🚀 How to Add a Partner

To add a new partner or update existing data, please follow these steps:

1. **Fork the repository** (or edit the file directly if you have write access).
2. Open the file `partners.json`.
3. Add a new object at the end of the list (remember the **comma** after the previous entry!).
4. Create a **Pull Request** with the partner's name as the title.

---

## 🛠 JSON Structure

Here is an example of a complete entry. Copy this block and customize it:

```json
{
  "name": "Community Name",
  "website_url": "https://example.com",
  "discord_name": "Username#0000",
  "discord_id": "123456789012345678",
  "server_id": "987654321098765432",
  "invite_url": "https://discord.gg/example",
  "description": "A short description of the partner community (max. 200 characters)."
}

```

### Fields Explained:

| Field | Type | Description |
| --- | --- | --- |
| `name` | String | The official name of the partner or organization. |
| `website_url` | String | Link to the official website (starting with `https://`). |
| `discord_name` | String | The Discord username of the primary contact person. |
| `discord_id` | String | The unique User ID of the contact person (must be a **String**!). |
| `server_id` | String | The unique ID of the partner's Discord server. |
| `invite_url` | String | A **permanent** Discord invite link. |
| `description` | String | A short summary of what makes the community special. |

---

## ⚠️ Important Notes

* **ID Format:** Please always enter Discord IDs (User & Server) in **quotation marks** (`"123..."`). This prevents systems from rounding long numbers incorrectly.
* **Invite Links:** Ensure that the Discord link is set to **"Never expire"**. Expired links will be automatically removed during the next audit.
* **Syntax Check:** A missing comma between objects `{...}` will cause the list to become unreadable. Use a JSON validator if you are unsure.

---

## 🎨 Integration

This data is automatically synchronized by our systems:

* **Discord Bot:** Posts partner embeds in the `#partners` channel.
* **Website:** Displays partner logos and descriptions in the footer.

---

## ⚖️ Rules of Conduct

* Only approved partnerships may be added to the `partners.json`.
* Maliciously deleting or altering entries of other partners will result in an immediate revocation of access rights.
