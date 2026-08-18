# Calculation Rush

> High-intensity, arcade-paced mental arithmetic conditioning engine designed for competitive management entrance examinations (CAT / XAT / GMAT / GRE).

**Live Application:** https://manandewan.github.io/calculationrush

---

## The Purpose

In competitive aptitude exams like CAT (Common Admission Test), knowing concepts, formulas, and problem-solving shortcuts is essential - but none of it matters if you cannot accurately and rapidly arrive at the final numerical answer.

When intermediate calculations (such as $37.5\% \text{ of } 240$, $19 \times 7$, or $28^2 - 22^2$) take 15-20 seconds on rough sheets, valuable time slips away and careless arithmetic errors cost marks.

Calculation Rush conditions your mental arithmetic into pure subconscious reflex through rapid, gamified, multi-topic hybrid sprints. It bridges the gap between knowing the concept and executing the final calculation with speed and accuracy under clock pressure.

---

## Core Features

### 1. 100% Dynamic On-The-Fly Question Engine
* **Infinite Replayability:** Zero static or hardcoded question banks. Every problem, operand, solution step, and distractor is generated algorithmically in real time.
* **Anti-Repetition Signature Cache:** Tracks the last 15 mathematical signatures to guarantee zero back-to-back duplicate questions.
* **No Isolated Drills:** Operations are combined into realistic hybrid expressions with addition and subtraction.

### 2. Cognitive "Ideal Time" Dynamic Benchmarking
Every generated question analyzes its own cognitive load (retrieval steps, operations, and intermediate terms) to compute an objective target completion time:
* **Squares ($1^2\text{--}30^2$):** $+1.2\text{s}$ to $+2.2\text{s}$
* **Cubes ($1^3\text{--}20^3$):** $+2.0\text{s}$ to $+3.2\text{s}$
* **Unit Fractions & Multiples ($\frac{1}{2}\text{--}\frac{1}{20}$):** $+1.8\text{s}$ to $+4.4\text{s}$
* **Factorial Ratios ($\frac{7!}{5!}$):** $+2.5\text{s}$ to $+4.5\text{s}$
* **Equal-Distance Product Twins ($(x-d)(x+d)$):** $+3.0\text{s}$ to $+4.5\text{s}$

### 3. Anti-Cheesing MCQ Distractor Traps
* Distractor options intentionally share identical unit digits ($\pm 10, \pm 20, \pm 50, \pm 100$ offsets).
* Eliminates the ability to cheese questions via unit-digit elimination; forces full mental computation.

### 4. Untimed "Retry Mistakes" Practice Mode
* Sprints log incorrect or skipped questions into an active mistake queue.
* Clicking Retry Mistakes launches an Untimed Stopwatch Mode allowing deep, deliberate decomposition of weak areas without clock pressure.

### 5. Local Analytics & Streak Tracking
* **Detailed Breakdown:** Accuracy %, Net Score ($+3$ for correct, $-1$ for wrong), Average Pace per Question, and Time Sinks.
* **Weak Area Detection:** Automatically tags categories where accuracy drops below 75%.
* **Local History Log:** Persists your last 25 sprint attempts in localStorage with individual delete and Clear All controls.

### 6. Interactive Spotlight Guide & Full Reference Dashboard
* **Interactive Spotlight Walkthrough:** 4-step live UI spotlight explaining duration, difficulty modes, topic selectors, and navigation.
* **Comprehensive Reference Deck:** High-speed lookup tables for:
  * Fractions ($\frac{1}{2}\text{ to }\frac{1}{20}$ and family multiples)
  * Squares ($1^2\text{ to }30^2$) & Cubes ($1^3\text{ to }20^3$)
  * Higher Powers (Bases 2, 3, 4, 5, 6, 7)
  * Factorials ($0!\text{ to }10!$)
  * Roots ($\sqrt{2}, \sqrt{3}, \sqrt{5} \dots \sqrt{10}$)
  * Multiplication Tables ($1\text{ through }30$)

---

## High-Yield CAT Calculation Patterns

The generator tests the following high-frequency patterns:

| Pattern | Expression Structure | Mental Technique |
| :--- | :--- | :--- |
| **Difference of Squares** | $(34^2 - 16^2) + 45$ | $(a-b)(a+b) \rightarrow 18 \times 50 = 900 + 45 = \mathbf{945}$ |
| **Equal-Distance Twins** | $(28 \times 32) + 45$ | $(30^2 - 2^2) = 900 - 4 = 896 + 45 = \mathbf{941}$ |
| **Base-50 / Base-100 Squaring** | $47^2 + 54$ | $(25 - 3)\times 100 + 3^2 = 2209 + 54 = \mathbf{2263}$ |
| **Percentage Reversals** | $(32\% \text{ of } 250) + 48$ | Reverse: $25\% \text{ of } 320 = 80 + 48 = \mathbf{128}$ |
| **$5/18$ & $18/5$ Conversion Arithmetic** | $(\frac{5}{18} \text{ of } 72) + 43$ | $(5 \times 4 = 20) + 43 = \mathbf{63}$ |
| **DILR Multi-Term Column Sums** | $47 + 68 + 84 + 39$ | Group tens & units: $(40+60+80+30) + (7+8+4+9) = \mathbf{238}$ |

---

## Architecture & Tech Stack

* **Zero Dependencies:** Built entirely with standard HTML5, CSS3 (Modern Glassmorphism & Custom Properties), and Vanilla JavaScript (ES6+).
* **Single File Architecture:** Zero asset build pipelines, zero npm bloating, 100% offline-first execution.
* **Instant Deployment:** Hosted directly on GitHub Pages.

```text
calculationrush/
└── index.html      # Complete standalone web application (UI, CSS styles, & JS engine)
└── README.md       # Comprehensive documentation
```

---

## Getting Started

### Option 1: Live Web App
Open **https://manandewan.github.io/calculationrush** directly on any desktop or mobile browser.

### Option 2: Mobile App Experience (PWA / Add to Home Screen)
1. Open the app link on iOS Safari or Android Chrome.
2. Tap Share -> "Add to Home Screen".
3. Launch directly from your home screen as a full-screen, distraction-free app.

### Option 3: Local Development
Clone and run with any static HTTP server:
```bash
git clone https://github.com/manandewan/calculationrush.git
cd calculationrush
python3 -m http.server 5173
```
Open `http://localhost:5173` in your browser.

---

## Recommended 100-Day Conditioning Routine

1. **Daily Anchor:** Do exactly one 15-Minute Sprint every morning before starting your regular CAT prep.
2. **First 14 Days (Adaptation):** Allow yourself to jot down only 1 intermediate anchor number on paper (e.g. holding `72` while computing `90`).
3. **Days 15-100 (Automaticity):** Drop pen and paper completely. Force mental left-to-right decomposition.
4. **Always Close the Loop:** Use the Retry Mistakes untimed mode after every session to eliminate misretrievals before logging off.

---

## License
MIT License. Free to use, adapt, and practice with for all competitive exam aspirants.
