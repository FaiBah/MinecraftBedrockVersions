# 🎮 Minecraft Bedrock Versions

> 📦 An automatically updated database of Minecraft Bedrock **Stable** and **Preview** versions.
>
> Version data is collected from [MCPELIFE](https://mcpelife.com/).

---

## 📦 Version Overview

| Type | Field | Description |
|:--|:--|:--|
| 🟢 Stable | `stable` | Latest stable version |
| 🔵 Preview | `preview` | Latest preview version |
| 📚 Stable History | `versions` | Stable version history |
| 🧪 Preview History | `preview_versions` | Preview version history |

<sub>Version lists are ordered from newest to oldest.</sub>

## 🔗 JSON Data

**File:** [`versions.json`](https://github.com/FaiBah/MinecraftBedrockVersions/blob/main/versions.json)

[📥 View Raw JSON](https://raw.githubusercontent.com/FaiBah/MinecraftBedrockVersions/main/versions.json)

<details>
<summary>📄 JSON Structure</summary>

```json
{
  "stable": "<latest-stable>",
  "preview": "<latest-preview>",
  "versions": [
    "<stable-version>",
    "<stable-version>",
    "<stable-version>"
  ],
  "preview_versions": [
    "<preview-version>",
    "<preview-version>",
    "<preview-version>"
  ]
}
```

</details>

---

## 🚀 Usage

**Requirement:** [jq](https://jqlang.github.io/jq/)

Base URL:
```text
https://raw.githubusercontent.com/FaiBah/MinecraftBedrockVersions/main/versions.json
```

### 🟢 Latest Stable

```bash
curl -s https://raw.githubusercontent.com/FaiBah/MinecraftBedrockVersions/main/versions.json | jq -r '.stable'
```

### 🔵 Latest Preview

```bash
curl -s https://raw.githubusercontent.com/FaiBah/MinecraftBedrockVersions/main/versions.json | jq -r '.preview'
```

### 📚 All Stable Versions

```bash
curl -s https://raw.githubusercontent.com/FaiBah/MinecraftBedrockVersions/main/versions.json | jq -r '.versions[]'
```

### 🧪 All Preview Versions

```bash
curl -s https://raw.githubusercontent.com/FaiBah/MinecraftBedrockVersions/main/versions.json | jq -r '.preview_versions[]'
```

---

## 🌐 Source

- [MCPELIFE](https://mcpelife.com/)
