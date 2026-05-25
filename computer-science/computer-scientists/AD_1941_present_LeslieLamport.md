# Leslie Lamport (1941– )
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

## 獨特的哲學：思維勝過程式碼

Lamport 一直強調：**「如果你沒有在思考，你就不算是在寫程式。」** 他極力推廣 **TLA+ (Temporal Logic of Actions)** 規格語言。他認為現代軟體災難的原因往往在於「思考不足」，直接動手寫程式碼而不先進行數學建模是非常危險的。

---

## "I'm not smart, I have the gift of abstraction..."

Lamport 的這句話展現了他將自身非凡成就歸功於「抽象化（abstraction）」能力而非純粹智商的謙遜與真知。這句話精準指出了軟體工程與分散式系統（distributed systems）的本質：透過建立精準的模型來簡化複雜度，而非靠硬寫硬記。

Lamport 作為圖靈獎（Turing Award）得主、分散式系統的奠基者，同時也是 LaTeX 的創造者，他說這句話絕非單純的客套，而是道出了計算機科學思考秘密。我們可以從以下幾個維度來解讀他的這番話：

### 1. 什麼是「抽象化的天賦」？

在計算機科學中，抽象化是指「剝離無關緊要的細節，只保留核心邏輯與本質特徵」的能力。 Lamport 認為自己並不比別人「聰明」（例如擁有過人的心算速度或記憶力），但他能看穿表象的混亂。

當大家都在探討特定的伺服器、網路線、作業系統漏洞時，Lamport 能將這些具體事物抽象化為時間戳記（timestamps）、邏輯時鐘（logical clocks）和狀態機（state machines）。著名的 **Lamport 時間戳記（Lamport timestamps）** 就是最典型的例子——他把複雜的物理時間同步問題，精煉成了一個極其簡潔的數學偏序關係（partial ordering）。

### 2. 「聰明」與「抽象化」的對立

- **傳統定義的「聰明」**： 往往擅長在極其複雜的環境中，靠著強大的大腦硬實力（如超高記憶力、同時處理多線程的 CPU 般大腦）硬幹出解決方案。

- **Lamport 的「抽象化」**： 則是拒絕進入複雜度泥潭。他的思維方式是：「既然這個問題太複雜，說明我的思考框架不對，我需要把它提升到一個更高的維度，讓複雜的問題在那裡變得顯而易見。」

這正如微軟研究院（Microsoft Research）同仁對他的評價：他總是能用最簡單的數學工具，去定義並解決最棘手的現實問題。

### 3. 這句話對軟體工程師的啟發

在現代軟體開發中，我們常常被各種新的框架、工具、API 版本搞得焦頭爛額。Lamport 的話提醒了我們：

卓越的工程師與平庸工程師的本質差別，不在於記住了多少語法或刻苦加班，而在於**能否從亂象中抽離出可重複利用的模型（models）與架構（architectures）**。

如果你覺得一個系統太過複雜、難以維護，往往不是因為你不夠聰明，而是因為缺乏正確的抽象。

### 結論

Lamport 這句話最迷人的地方在於，它將一個看似高不可攀的「科學巨擘形象」拉回到了本質的思考方法上。他告訴大眾：看透本質。 這不僅僅是他的天賦，更是他送給所有程式設計師與科學研究者的思維指南。

---