<div align="center">

<img src="./banner.svg" alt="BST Playground — see binary search tree operations animate" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=19&duration=2600&pause=900&color=FBBF24&center=true&vCenter=true&width=700&height=40&lines=%F0%9F%8C%B3+Type+a+number.+Watch+it+find+its+place.;%F0%9F%94%8D+Search%2C+insert%2C+delete+%E2%80%94+step+by+step;%F0%9F%9A%B6+In-order%2C+pre-order%2C+post-order%2C+level-order;%F0%9F%A7%A9+Built+while+cracking+LeetCode+1569" alt="typing intro"/>

<p>
<img src="https://img.shields.io/badge/status-in_development-F5B841?style=for-the-badge" alt="status"/>
<img src="https://img.shields.io/badge/runs_in-your_browser-FBBF24?style=for-the-badge" alt="browser"/>
<img src="https://img.shields.io/badge/install-nothing-F472B6?style=for-the-badge" alt="no install"/>
</p>
<p>
<img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML"/>
<img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white" alt="CSS"/>
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JS"/>
<img src="https://img.shields.io/badge/SVG-animations-FFB13B?style=flat-square&logo=svg&logoColor=black" alt="SVG"/>
<img src="https://img.shields.io/badge/license-MIT-blue?style=flat-square" alt="MIT"/>
</p>

**[🌐 Open the playground](https://hemashreevi.github.io/bst-playground/)** · **[✨ Features](#-features)** · **[🧠 What you'll learn](#-what-youll-learn)** · **[🗺️ Roadmap](#%EF%B8%8F-roadmap)**

</div>

---

## 💡 Why?

Binary search trees look simple on paper, until you have to **delete a node with two children** or work out **how many insert orders build the same tree**. Static diagrams don't show *how* the tree changes.

**BST Playground animates every comparison and every pointer move**, so you can see the algorithm instead of imagining it.

## ✨ Features

<table>
<tr>
<td width="33%" align="center">➕<br/><b>Animated insert</b><br/><sub>Watch the value compare its way down: smaller goes left, bigger goes right</sub></td>
<td width="33%" align="center">🗑️<br/><b>All 3 delete cases</b><br/><sub>Leaf, one child, and two children with the in-order successor highlighted</sub></td>
<td width="33%" align="center">🔍<br/><b>Search trace</b><br/><sub>The path lights up and shows how many steps it took</sub></td>
</tr>
<tr>
<td align="center">🚶<br/><b>4 traversals</b><br/><sub>In, pre, post and level order, walked node by node</sub></td>
<td align="center">⏯️<br/><b>Step mode</b><br/><sub>Pause, step forward or back, change speed, with a plain-English explanation of each step</sub></td>
<td align="center">🧩<br/><b>LeetCode 1569 mode</b><br/><sub>Count the insert orders that build the <i>same</i> tree, and see why</sub></td>
</tr>
<tr>
<td align="center">📏<br/><b>Live stats</b><br/><sub>Height, node count, balanced or skewed, and Big-O for each operation</sub></td>
<td align="center">🎲<br/><b>Quick builds</b><br/><sub>Paste an array, generate a random tree, or a worst-case sorted one</sub></td>
<td align="center">☕<br/><b>Java code panel</b><br/><sub>The matching Java code, with the running line highlighted</sub></td>
</tr>
</table>

## 🎬 Demo

> 🛠️ *GIFs of insert, delete and traversal go here once they're built.*

## 🧠 What you'll learn

| Operation | Average | Worst (skewed tree) | Shown in the playground |
|---|:-:|:-:|---|
| Search | `O(log n)` | `O(n)` | path highlight and step counter |
| Insert | `O(log n)` | `O(n)` | compare-and-descend animation |
| Delete | `O(log n)` | `O(n)` | successor swap, visualised |
| Traversal | `O(n)` | `O(n)` | node-by-node walk |

```mermaid
flowchart TD
    S["insert(x)"] --> C{"x < node?"}
    C -- "yes" --> L["go left"]
    C -- "no" --> R["go right"]
    L --> E{"empty spot?"}
    R --> E
    E -- "yes" --> P["🌱 place x here"]
    E -- "no" --> C
```

## ⚡ Run locally

```bash
git clone https://github.com/HemashreeVI/bst-playground.git
cd bst-playground
python -m http.server 8000     # then open http://localhost:8000
```

## 🗂️ Project structure

```
bst-playground/
├── index.html      # layout and controls
├── style.css       # theme and animations
├── bst.js          # the tree: insert, delete, search, traversals
├── render.js       # draws and animates the tree in SVG
└── lc1569.js       # "number of ways to reorder" mode
```

## 🗺️ Roadmap

- [ ] **Step 1:** Draw a tree from an array
- [ ] **Step 2:** Animated insert and search
- [ ] **Step 3:** Delete, all three cases
- [ ] **Step 4:** Four traversals with step mode
- [ ] **Step 5:** LeetCode 1569 mode and the Java code panel
- [ ] *Stretch:* AVL rotations, shareable tree links

## 🧰 Built with

<p align="center"><img src="https://skillicons.dev/icons?i=html,css,js,java,github&theme=dark" alt="tech"/></p>

---

<div align="center">

**Built by [Hemashree V I](https://hemashreevi.github.io)** while learning BSTs from zero 🌳

<a href="https://hemashreevi.github.io"><img src="https://img.shields.io/badge/Portfolio-8B5CF6?style=flat-square&logo=googlechrome&logoColor=white" alt="Portfolio"/></a>
<a href="https://www.linkedin.com/in/hema-shree-373622289"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="mailto:shreejith2005@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email"/></a>

</div>
