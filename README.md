# DSA 1 — Interactive CS & Algorithm Visualizers

An interactive collection of self-contained web applications designed to teach fundamental computer science concepts, algorithmic reasoning, and problem-solving strategies through visual simulation.

Every module is completely standalone—built using vanilla HTML, CSS/Tailwind, and JavaScript with no build steps, bundlers, or package dependencies required.

---

## 📦 Included Modules

### 1. Traffic Light Abstraction (`/traffic-light`)
* **Core Concept:** Levels of abstraction and state machines.
* **What it does:** Features an interactive slider that strips away real-world noise across four distinct levels: realistic intersection physics → schematic wireframe → finite state machine (FSM) → pure algorithmic execution loop.

### 2. Traffic Light Phase Planning (`/graph-coloring-presentation` & `/graph-coloring-puzzle`)
* **Core Concept:** Graph modeling, conflict graphs, and greedy graph coloring.
* **Presentation Mode:** An automated and step-by-step walkthrough showing how non-conflicting traffic paths are assigned shared signal phases using minimal colors.
* **Puzzle Mode:** An interactive challenge where users assign phase colors across intersection conflict nodes and validate whether any traffic collisions occur.

### 3. The Marble Jar (`/marble-game`)
* **Core Concept:** Invariant principles, loop invariants, and algorithm termination.
* **What it does:** Breaks down the classic two-color marble reduction puzzle. Instead of brute-forcing an exponential state tree ($3^n$ paths), it interactively demonstrates how tracking parity invariants guarantees the final state, while contrasting it with non-terminating loops.

### 4. Demystifying Big-O Time Complexity (`/time-complexity`)
* **Core Concept:** Asymptotic analysis, runtime growth rates, and algorithm classification.
* **What it does:** An interactive slide deck framed around a facility manager unlocking doors with a key ring:
  * **$O(1)$ Constant Time:** Tagged master keys (direct index access).
  * **$O(n)$ Linear Time:** Sequential key testing (linear scan, best/average/worst case).
  * **$O(\log n)$ Logarithmic Time:** Ordered numbered keys using binary search and recursive halving.
  * **$O(n^2)$ Quadratic Time:** All-pairs key-to-door testing (nested iterations).
  * **Interactive Arena:** Dynamic graphs and sliders comparing operations as input size $N$ scales.

### 5. Peanut Butter Sandwich Maker (`/sandwich-maker`)
* **Core Concept:** Algorithmic precision, preconditions, postconditions, and side effects.
* **What it does:** A canvas-based interactive simulation of the classic CS instruction exercise. Includes a natural-language parser that interprets plain-English commands (e.g., `"take slice"`, `"dip knife"`, `"spread"`) and exposes edge cases when commands are vague, out of order, or missing necessary preconditions.

---

## 🛠️ Tech Stack & Design

* **Zero Dependencies:** Pure vanilla JavaScript, HTML5 Canvas, and SVG.
* **Styling:** Modern CSS layouts and utility classes via Tailwind CSS CDN.
* **Web Audio API:** Real-time synthesized audio effects generated directly in code without external audio assets.
* **Responsive & Touch-Ready:** Optimized for desktops, tablets, and mobile devices.

---

## 🚀 Getting Started

Since all modules are static single-page applications, you can run them without installing Node.js or running a build pipeline.

### Option 1: Direct File Access
Simply navigate into any module directory and open `index.html` in your web browser:
```bash
# Example
open time-complexity/index.html
