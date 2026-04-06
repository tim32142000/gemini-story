# Leslie Lamport (1941-)
> 「分散式系統就是當你甚至不知道它存在的某台電腦壞了，會導致你自己的電腦無法工作。」  
> "A distributed system is one in which the failure of a computer you didn't even know existed can render your own computer unusable."  
> —— Leslie Lamport

<p align="left">
  <img src="https://upload.wikimedia.org/wikipedia/commons/5/50/Leslie_Lamport.jpg" width="300" alt="Lamport in 2008">
  <br>
  Lamport in 2008
  <br><i>
  By Leslie Lamport - <a rel="nofollow" class="external free" href="https://web.archive.org/web/20080809045739/http://lamport.org/">https://web.archive.org/web/20080809045739/http://lamport.org/</a>Source of original version: <a rel="nofollow" class="external free" href="https://web.archive.org/web/20030204122708/http://lamport.org/">https://web.archive.org/web/20030204122708/http://lamport.org/</a>, Copyrighted free use, <a href="https://commons.wikimedia.org/w/index.php?curid=487587">Link</a>
  </i>
</p>
<br><br>

## 從物理學到分散式系統的傳奇

Leslie Lamport 是一位對現代計算機科學，特別是**分散式系統 (Distributed Systems)** 有著決定性貢獻的學者。他的故事展現了如何將嚴謹的數學邏輯與物理直覺結合，解決數位世界中最混沌的順序問題。

---

## 成就與背景

* **貢獻：** 定義了分散式系統中「時間」與「順序」的本質，發明 **Paxos 演算法** 以及排版軟體 **LaTeX**。
* **學術背景：** 1960 年畢業於麻省理工學院 (MIT) 數學系，隨後於布蘭戴斯大學 (Brandeis University) 取得數學碩士與博士學位。
* **最高榮譽：** 2013 年榮獲計算機科學界最高獎項——**圖靈獎 (Turing Award)**。

---

## 關鍵人生階段與故事

### 1. 從數學與物理邁向計算機科學
Lamport 最初受的是正統數學訓練，這使他在面對計算機問題時，習慣以**形式化邏輯 (Formal Logic)** 的角度切入。他對問題的看法非常獨特：他認為程式碼不只是指令，而是一種數學對象。

### 2. 重新定義「時間」：邏輯時鐘 (Logical Clocks)
在 1978 年，他發表了著名的論文 *Time, Clocks, and the Ordering of Events in a Distributed System*：
* **背景：** 在多台電腦組成的系統中，每台機器的硬體時鐘都不精準。若 A 機器說現在是 10:00，B 機器說是 10:01，該如何判斷事件先後？
* **突破：** 他提出不需要依賴物理時間，而是透過訊息交換建立**因果關係 (Causality)**。這就是「Lamport 時鐘」，奠定了現代雲端運算的邏輯基礎。

### 3. 拜占庭將軍問題 (Byzantine Generals Problem)
Lamport 與同事提出了這個經典比喻，描述在可能有錯誤或惡意節點的網路中，如何達成一致性 (Consensus)。這項研究直接啟發了後來區塊鏈與加密貨幣的共識機制。

### 4. 幽默的 Paxos 演算法
Lamport 帶有一種知識分子的幽默。當他發明解決一致性問題的 **Paxos 演算法** 時，他虛構了一個名為 "Paxos" 的古希臘島嶼，描述島上的兼職議會如何投票。
* **趣聞：** 因為寫得太像考古小說，當時的同僚大多看不懂，論文被擱置了數年才被重新發現其巨大的價值。

### 5. LaTeX 的誕生
在 1980 年代初期，為了撰寫數學公式豐富的論文，他在 Donald Knuth 開發的 $TeX$ 基礎上，編寫了一套巨集 (Macros)，這就是現今學術界通用的 **LaTeX**。他曾自嘲開發 LaTeX 只是為了讓自己寫論文更方便。

---

## 獨特的哲學：思維勝過代碼

Lamport 一直強調：**「如果你沒有在思考，你就不算是在寫程式。」** 他極力推廣 **TLA+ (Temporal Logic of Actions)** 規格語言。他認為現代軟體災難的原因往往在於「思考不足」，直接動手寫程式碼而不先進行數學建模是非常危險的。

