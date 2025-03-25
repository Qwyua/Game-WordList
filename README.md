<h1 align="center">Gartic Word List</h1>
<h3 align="center">A Comprehensive Multi-Language Word List for the Gartic Game</h3>
<p align="center">
  <img height="210" src="./images/logo.png" alt="Project Logo">
</p>

_Enhance your Gartic experience with a detailed, multilingual word list to support players worldwide._

## 📌 **Project Overview**  

**Gartic Word List** aims to provide an extensive, organized, and easy-to-use word list for **Gartic** developers. This list includes words in multiple languages, enhancing gameplay and making it more enjoyable for all players. The word list will continuously evolve and improve through contributions, ensuring players from different parts of the world can enjoy a localized experience.

### Key Features
- **Multilingual Support**: The project supports various languages, providing words for each.
- **Regular Updates**: The word list is regularly updated to add more words and improve accuracy.
- **Community-driven**: Anyone can contribute to the project by adding new words or suggesting improvements.

---

### ❗Gartic WordList - Important Notice

This project collects words directly from Gartic's internal database. Some words may be incorrect or unrelated, but they originate from the game itself.

⚠️ We do not manually modify words. If you find incorrect words, report them to **team@gartic.com**.

🔹 For contributions, follow the guidelines in [CONTRIBUTING.md](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/.github/CONTRIBUTING.md).   
🔹 Fork the repository if you want to make improvements.   
🔹 We appreciate feedback, but we cannot change the game's word list.   

Thank you for your understanding!

---
## 🌍 **Languages Supported**

The project currently supports the following languages. For each language, an estimate of the total number of words included is provided:


| Language      | Word Count | Update |
|---------------|------------|-------------------|
| **[Portuguese](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Portuguese)**| 11510+ | Mar 10, 25 |
| **[English](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/English)**    | 7908+         ||
| **[Spanish](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Spanish)**   | 5793+          ||
| **[Italian](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Italian)**   | 5607+          ||
| **[French](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/French)**    | 5526+          ||
| **[Turkish](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Turkish)**   | 3067+          ||
| **[Indonesian](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Indonesian)**| 2720+          ||
| **[Chinese](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Chinese)**   | 2607+          ||
| **[Thai](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Thai)**      | 1874+          ||
| **[Czech](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Czech)**     | 1691+          ||
| **[Russian](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Russian)**   | 1441+          ||
| **[Bulgarian](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Bulgarian)** | 1235+          ||
| **[Dutch](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Dutch)**     | 1222+          ||
| **[Arabic](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Arabic)**    | 1181+          ||
| **[Korean](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Korean)**    | 1055+          ||
| **[Polish](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Polish)**    | 951+          ||
| **[German](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/German)**    | 950+          ||
| **[Vietnamese](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Vietnamese)**| 817+          ||
| **[Slovak](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Slovak)**    | 752+          ||
| **[Azerbaijani](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Azerbaijani)**| 500+         ||
| **[Romanian](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Romanian)**  | 460+          ||
| **[Hebrew](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Hebrew)**    | 423+          ||
| **[Hungarian](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Hungarian)** | 400+          ||
| **[Persian](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Persian)**   | 381+          ||
| **[Japanese](https://github.com/Gartic-Developers/Gartic-WordList/tree/main/languages/Japanese)**  | 367+          ||

> **Note**: The numbers above represent an approximate count of words for each language. These numbers may change as the project is updated.

---

# 📌 Gartic WordList API (for Developers)

Welcome to the **Gartic WordList API**! This project provides an easy way to fetch word lists for Gartic rooms using a simple JavaScript function.

## 🚀 How to Use?

### 1️⃣ Adding the Library
To use `getWordList`, you need to load the script dynamically. You can do this in two ways:

#### Option 1: Using Fetch & Eval (Recommended)
```js
fetch("https://cdn.jsdelivr.net/gh/Gartic-Developers/Gartic-WordList/src/getWordList.min.js").then((t=>t.text())).then((js=>eval(js)));
```

#### Option 2: Adding a Script Tag
```js
const script = document.createElement("script");
script.src = "https://cdn.jsdelivr.net/gh/Gartic-Developers/Gartic-WordList/src/getWordList.min.js";
document.body.appendChild(script);
```

### 2️⃣ Fetching Word Lists
You can retrieve word lists in two different ways:

#### Method 1: Using a Room Code
```js
const words = getWordList("324qc3");
console.log(words); // ["tofu", "vinaigrette", "meat", "parsley", "burrito", ...] 
```
This method extracts language and theme from the given code and fetches the corresponding word list.

#### Method 2: Using a Direct URL
```js
const words = getWordList("https://cdn.jsdelivr.net/gh/Gartic-Developers/Gartic-WordList/languages/English/foods.json");
console.log(words); // ["tofu", "vinaigrette", "meat", "parsley", "burrito", ...] 
```
This method fetches word lists directly from a valid GitHub repository URL.


## 🌍 Contribution
If you would like to contribute, please check out our repository: [CONTRIBUTING.md](https://github.com/Gartic-Developers/Gartic-WordList/blob/main/.github/CONTRIBUTING.md)

Happy coding! 🎨🚀

---

## 🤝 Contributors  

We extend our heartfelt gratitude to the amazing people who have contributed to this project! 💖  

<p align="center">
    <a href="https://github.com/KutayX7">
    <img src="https://github.com/KutayX7.png" width="80" height="80" style="border-radius: 50%;" alt="KutayX7">
  </a>
  <a href="https://github.com/NOXY-JS">
    <img src="https://github.com/NOXY-JS.png" width="80" height="80" style="border-radius: 50%;" alt="NOXY-JS">
  </a>
  <a href="https://github.com/ygnJavascript">
    <img src="https://github.com/ygnJavascript.png" width="80" height="80" style="border-radius: 50%;" alt="ygnJavascript">
  </a>
  <a href="https://github.com/Qwyua">
    <img src="https://github.com/Qwyua.png" width="80" height="80" style="border-radius: 50%;" alt="Qwyua">
  </a>
</p>

<p align="center">
  <a href="https://github.com/Gartic-Developers/Gartic-WordList/graphs/contributors">
    <img src="https://img.shields.io/github/contributors/Gartic-Developers/Gartic-WordList?color=blue&style=for-the-badge">
  </a>
</p>

<p align="center">
  <a href="https://github.com/Gartic-Developers/Gartic-WordList/graphs/contributors">
    <b>View All Contributors</b>
  </a>
</p>

