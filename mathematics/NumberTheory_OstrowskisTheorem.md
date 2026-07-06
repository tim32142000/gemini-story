# Ostrowski's theorem

**Ostrowski's theorem （奧斯特洛夫斯基定理）** 是數論中的一項基礎定理，它指出所有非平凡的賦值（valuation）對於有理數體 $\mathbb{Q}$ 而言，皆等價於標準的絕對值（Archimedean）或是 $p$-adic 絕對值（non-Archimedean）。

---

## 定理定義

對於有理數體 $\mathbb{Q}$ 上的任何非平凡絕對值 $|\cdot|$，它必屬於以下兩類之一：

1. **實絕對值（Archimedean valuation）**：  
存在一個 $0 < \alpha \le 1$，使得 $|x| = |x|_\infty^\alpha$。其中 $|x|_\infty$ 是常見的實數絕對值（即 $|x|_\infty = \max(x, -x)$）。

2. **$p$-adic 絕對值（Non-Archimedean valuation）**：  
存在一個質數 $p$，以及一個常數 $c > 1$，使得 $|x| = c^{-v_p(x)}$。其中 $v_p(x)$ 是 $p$-adic 指數（$x = p^k \frac{a}{b}$，其中 $p \nmid a, b$，則 $v_p(x) = k$）。

## 性質比較

### 實絕對值 ($|\cdot|_\infty$)
- 分類：Archimedean  
- 三角不等式：$|x+y| \le |x| + |y|$  
- 拓撲結構：連續、聯通  
- 完備化空間：$\mathbb{R}$  

### $p$-adic 絕對值 ($|\cdot|_p$)
- 分類：Non-Archimedean  
- 三角不等式：強三角不等式 $|x+y| \le \max(|x|, |y|)$  
- 拓撲結構：不連續、完全不聯通 (Totally disconnected)  
- 完備化空間：$\mathbb{Q}_p$  


## 重要意義

- **完備化（Completion）**： 此定理確立了 $\mathbb{Q}$ 的所有完備化空間只有兩種可能：實數體 $\mathbb{R}$ 與 $p$-adic 數體 $\mathbb{Q}_p$。這在代數數論（Algebraic Number Theory）中至關重要，因為它奠定了局部體（Local Fields）研究的基礎。  

- **Hasse 原理**： 許多數論問題（如二次型的解）可以先在所有的局部體（所有 $|\cdot|_p$ 及 $|\cdot|_\infty$）上進行檢驗，若在所有地方都有解，則在全體 $\mathbb{Q}$ 上也有解。這就是所謂的「局部-全域原則」（Local-Global Principle）。

---

