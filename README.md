# json-to-table-mui

A lightweight React component to render JSON data as a responsive Material UI table with built-in pagination, sorting, and search.

[![npm version](https://img.shields.io/npm/v/json-to-table-mui.svg)](https://www.npmjs.com/package/json-to-table-mui)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## ✨ Features

- ✅ Automatically generates table from any JSON array
- 🔍 Built-in search filter
- 🔃 Column sorting (ascending/descending)
- 📄 Pagination controls
- 🎨 Uses [Material UI v5](https://mui.com/)
- 🧠 TypeScript support included

---

## 🚀 Installation

```bash
npm install json-to-table-mui
```

Or with yarn:

```bash
yarn add json-to-table-mui
```

---

## 📦 Usage

```tsx
import React from "react";
import JsonToTable from "json-to-table-mui";

const data = [
  { name: "Alice", age: 25, country: "USA" },
  { name: "Bob", age: 30, country: "Canada" },
];

export default function App() {
  return (
    <div>
      <h1>My Table</h1>
      <JsonToTable data={data} />
    </div>
  );
}
```

---

## 📐 Props

| Prop   | Type    | Description                      |
| ------ | ------- | -------------------------------- |
| `data` | `any[]` | Array of JSON objects to display |

---

## 🛠 Dev Setup

```bash
git clone https://github.com/yourusername/json-to-table-mui
cd json-to-table-mui
npm install
npm run dev     # Starts Vite demo in /example
npm run build   # Builds library to /dist
```

---

## 📄 License

[MIT](LICENSE)

---

## 🙌 Contributing

Pull requests and stars are welcome!  
Please open an issue first if you want to add a feature or report a bug.
