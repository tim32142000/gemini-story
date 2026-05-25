# Curry–Howard correspondence

Curry–Howard 對應（Curry–Howard correspondence）描述了計算機程式與數學邏輯之間的深刻聯繫，簡而言之，這是一個「程式即證明，類型即命題」（Programs are proofs, Types are propositions）的架構，徹底改變了計算機科學與數理邏輯的發展。

---

### 故事的開端：兩種邏輯的相遇

Curry–Howard 對應並非由某一個人單獨在一個下午發明，而是由兩位邏輯學家在不同時間、不同領域的工作，最終被後人匯聚而成的思想結晶。

#### 1. Haskell Curry 與組合子邏輯 (1930年代)

美國數學家 Haskell Curry 在研究「組合子邏輯」（Combinatory Logic）時發現，某些邏輯公理的變換形式，與特定類型的函式計算結構驚人地相似。他意識到，邏輯的推導規則似乎對應於計算結構中的變換步驟。

#### 2. William Alvin Howard 與自然演繹 (1960年代)

1969年，數學家 William Alvin Howard 在一份手稿中，明確展示了「自然演繹」（Natural Deduction，一種邏輯證明系統）與「型別化 lambda 演算」（Typed Lambda Calculus，一種計算模型）之間的同構關係（Isomorphism）。他證明了只要你寫出一個程式，你其實就是在寫一個邏輯證明。

### 為什麼這很重要？

Curry–Howard 對應的核心在於將兩個原本看似無關的領域劃上等號：

| 邏輯學 (Logic) | 計算機科學 (Computer Science) |
| :--- | :--- |
| 命題 (Proposition) | 類型 (Type) |
| 證明 (Proof) | 程式 (Program / Term) |
| 邏輯聯結詞 (Implication $\rightarrow$) | 函式類型 (Function type $A \rightarrow B$) |
| 連言 (Conjunction $\wedge$) | 乘積型別 (Product type / Tuple) |
| 選言 (Disjunction $\vee$) | 和型別 (Sum type / Either) |

### 這個發現改變了什麼？

這個對應關係不僅僅是理論上的樂趣，它為現代計算機科學帶來了革命性的工具：

- **自動化定理證明器（Automated Theorem Provers）**： 如 Coq、Lean 或 Agda。在這些系統中，程式設計師寫出的程式如果不通過編譯器檢查，就代表邏輯證明不成立。這使得人類可以確信程式是「絕對正確」的（Formal Verification）。

- **強型別程式語言的發展**： 許多現代程式語言（如 Haskell, Rust）的型別系統之所以強大，其底層靈感都深受 Curry–Howard 對應影響。當你編寫強型別程式時，你實際上是在建立一個邏輯系統，確保不會發生執行期錯誤（Runtime error）。

- **程式語言設計的統一**： 它架起了橋樑，讓電腦科學家可以用處理邏輯問題的方法來優化程式，也可以用程式結構來尋找邏輯中的漏洞。

### 結語

Curry–Howard 對應告訴我們，**計算與推理是同源的**。當你編寫出一個能夠編譯通過的複雜函式時，你其實已經完成了一個優雅的邏輯證明。這是一個將「運算」提升至「真理」層次的深刻洞見，至今仍是計算機科學理論中優美的篇章。

---