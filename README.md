# zero-tags - #0, %230

**zero-tags** is a type-safe TypeScript library for working with a **massive collection of standardized and well-defined tags**. It supports powerful features like **grouped tags**, **alias tags**, and flexible **searching and filtering tooling** — all with full TypeScript support for enhanced developer experience.

---

## ✨ Features

- ✅ **Standardized Tags**  
  A large, curated set of tags with clear definitions and consistent naming conventions.

- 🏷 **Grouped Tags**  
  Organize tags into logical groups for better structure and semantic meaning.

- 🪞 **Alias Tags**  
  Use alternative names or synonyms for tags to improve discoverability and interoperability.

- 🔍 **Search & Filter Tooling**  
  Built-in utilities for searching, filtering, and matching tags with high performance.

- 🧠 **Type-Safe API**  
  Written in TypeScript with full type safety and IDE support — no more typos or guesswork.

---

## 📦 Installation

```bash
npm install @zeroopensource/zero-tags
# or
yarn add @zeroopensource/zero-tags
# or
pnpm add @zeroopensource/zero-tags
```

---

## 🚀 Quick Start

```ts
import { getTag, searchTags, filterTags, TAGS } from 'zero-tags'

// Get a tag definition
const tag = getTag('machine-learning')

// Search for tags
const results = searchTags('ai') // returns relevant tag matches

// Filter tags by group
const aiTags = filterTags({ group: 'Artificial Intelligence' })

// Use tag aliases
const sameTag = getTag('ml') // resolves to 'machine-learning' tag
```

---

## 🧩 Tag Structure

Each tag follows a consistent structure:

```ts
type Tag = {
  id: string // Unique identifier, e.g., "machine-learning"
  name: string // Human-readable name
  description?: string // Optional description
  group?: string // Optional group/category
  aliases?: string[] // Optional list of alias strings
}
```

---

## 📚 Usage Scenarios

- Content categorization
- Metadata tagging for files, documents, or media
- Building tag-based filters in apps
- Enhancing search relevance
- Semantic data organization

---

## 🛠 Tooling API

| Function                | Description                   |
| ----------------------- | ----------------------------- |
| `getTag(id)`            | Get a tag by its ID or alias  |
| `searchTags(query)`     | Search for tags by keyword    |
| `filterTags({ group })` | Get tags by group             |
| `allTags()`             | Returns the full list of tags |

---

## 📁 Project Structure

```
zero-tags/
├── src/
│   ├── tags/           # Tag definitions
│   ├── groups/         # Group organization
│   ├── aliases/        # Alias handling
│   └── utils/          # Tooling functions (search, filter, etc.)
├── index.ts
└── README.md
```

---

## 🤝 Contributing

We welcome contributions! Feel free to open issues, suggest new tags, or improve tooling.

```
git clone https://github.com/zeroopensource/zero-tags
cd zero-tags
pnpm install
pnpm dev
```

---

## License

MIT © 2025 Zero Open Source™ (aka ZeroOpenSource™; "Zero")

See [LICENSE](LICENSE) for more details.

---

## 🧠 About

**zero-tags** is part of the [Zero Open Source](https://github.com/zeroopensource) ecosystem — building clean, modular, and well-documented tools for modern developers.
