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
import React from 'react';
import ReactDOM from 'react-dom/client';
import JsonToTable from '../../../NPM Projects/json-to-table-mui/src/JsonToTable';

const sampleData = [
  { name: 'Alice', age: 25, country: 'USA' },
  { name: 'Bob', age: 30, country: 'Canada' },
  { name: 'Charlie', age: 22, country: 'UK' },
  { name: 'David', age: 28, country: 'Germany' },
  { name: 'Eva', age: 35, country: 'France' },
  { name: 'Frank', age: 27, country: 'Italy' },
  { name: 'Grace', age: 31, country: 'Spain' },
  { name: 'Helen', age: 26, country: 'Australia' },
];

const App = () => {

  const onRowClicked = (row: any) => {
      console.log("row", row);
  }
  return(<>
  <div style={{ padding: 20 }}>
    <h1>json-to-table-mui Demo</h1>
    <JsonToTable
      data={sampleData}
      onFirstValueClick={(row:any) => onRowClicked(row)}
    />
  </div>
  </>
  )
};

export default App;

const root = ReactDOM.createRoot(document.getElementById('root')!);
root.render(<App />);

```

---

## 📐 Props

| Prop                | Type                 | Description                       |
| ------------------- | -------------------- | --------------------------------  |
| `data`              | `any[]`              | Array of JSON objects to display  |
| ------------------- | -------------------- | --------------------------------- |
| `onFirstValueClick` | `(row: any) => void` | Called when the first JSON field  |
|                     |                      | value of a row is clicked
---

## 🛠 Dev Setup

```bash
git clone https://github.com/jfsemideys/json-to-table-mui
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
