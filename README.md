# 計概 排序報告

* [cite_start]**學號** : 11428122 [cite: 1]
* [cite_start]**姓名** : 林暐鈞 [cite: 2]
* [cite_start]**模擬頁面** : [https://jetercycu.github.io/soft_homework/](https://jetercycu.github.io/soft_homework/) [cite: 3]

---

## [cite_start]一、 氣泡排序法 (Bubble Sort) [cite: 4]

### [cite_start]1. 簡述原理 [cite: 5]
[cite_start]氣泡排序法是一種簡單的交換排序。 [cite: 6] [cite_start]一次比較兩個相鄰的元素，如果它們的順序錯誤（例如：前面的數字大於後面的數字），就將它們交換過來。 [cite: 6] [cite_start]這個過程會重複進行，直到不再需要交換為止。 [cite: 6] [cite_start]因為越大的元素會經由交換慢慢「浮」到數列的頂端（尾部），故名氣泡排序。 [cite: 6]

### [cite_start]2. 複雜度分析 [cite: 7]
* [cite_start]**最佳時間複雜度**： O(N) （當資料已經是排序好的狀態，只需走訪一次且無交換）。 [cite: 8]
* [cite_start]**最壞 / 平均時間複雜度**： O(N^2) [cite: 9]

### [cite_start]3. 模擬實作內容 [cite: 10]
[cite_start]在測試中，我們輸入了 100,000 和 10000 個完全倒序的整數。 [cite: 11] [cite_start]因為平均時間複雜度為 O(N^2) 所以當要排序的數量差 10 倍時，所花的時間是 100 倍。 [cite: 11]

---

## [cite_start]二、 選擇排序法 (Selection Sort) [cite: 12]

### [cite_start]1. 簡述原理 [cite: 13]
[cite_start]選擇排序法的核心思想是「尋找極值」。 [cite: 14] [cite_start]它將數列分為「已排序」與「未排序」兩個區間。 [cite: 14] [cite_start]每次會從未排序區間中掃描找出最小值（或最大值），然後將它與未排序區間的第一個元素交換位置。 [cite: 14] [cite_start]這個過程會重複進行，直到所有元素都進入已排序區間。 [cite: 14] [cite_start]選擇排序對資料的初始狀態不敏感，即使給定其他排列方式，比較次數依然固定，時間增幅比例不變。 [cite: 14]

### [cite_start]2. 複雜度分析 [cite: 15]
* [cite_start]**最佳時間複雜度**：(N^2)（無論資料初始狀態為何，都必須執行完整掃描）。 [cite: 16]
* [cite_start]**最壞 / 平均時間複雜度**：O(N^2) [cite: 17]

### [cite_start]3. 模擬實作內容 [cite: 18]
[cite_start]在測試中，我們輸入了 100,000 和 10,000 個完全倒序的整數。 [cite: 19] [cite_start]因為平均時間複雜度為 $O(N^2)$，所以當要排序的數量差 10 倍時，所花的時間是 100 倍。 [cite: 19]

---

## [cite_start]三、 插入排序法 (Insertion Sort) [cite: 20]

### [cite_start]1. 簡述原理 [cite: 21]
[cite_start]插入排序法的運作方式類似於整理手牌。 [cite: 22] [cite_start]它同樣將數列分為「已排序」和「未排序」兩部分。 [cite: 22] [cite_start]每次從未排序的區間取第一個元素，由後往前掃描已排序的區間，找到合適的位置後將其插入，並將較大的元素往後平移以騰出空間。 [cite: 22]

### [cite_start]2. 複雜度分析 [cite: 23]
* [cite_start]**最佳時間複雜度**：O(N)（當資料已經是排序好的狀態，每次只需比較一次即可完成該回合）。 [cite: 24]
* [cite_start]**最壞 / 平均時間複雜度**：O(N^2) [cite: 25]

### [cite_start]3. 模擬實作內容 [cite: 26]
[cite_start]在測試中，我們輸入了 100,000 和 10,000 個完全倒序的整數。 [cite: 27] [cite_start]因為倒序正好是插入排序的最壞情況，平均與最壞時間複雜度皆為 (N^2)，所以當要排序的數量差 10 倍時，所花的時間同樣是 100 倍。 [cite: 27]

---

## [cite_start]四、 合併排序法 (Merge Sort) [cite: 28]

### [cite_start]1. 簡述原理 [cite: 29]
[cite_start]合併排序法採用「分治法 (Divide and Conquer)」策略。 [cite: 30] [cite_start]它會將原本的陣列不斷對半拆分，直到每個子陣列只剩下 1 個元素（視為已排序）。 [cite: 30] [cite_start]接著，將相鄰的兩個已排序子陣列，依序比較大小並合併成一個較大的已排序陣列，重複此動作直到全部合併完成。 [cite: 30]

### [cite_start]2. 複雜度分析 [cite: 31]
* [cite_start]**最佳時間複雜度**：O(N log N) [cite: 32]
* [cite_start]**最壞 / 平均時間複雜度**：O(N log N) [cite: 33]

### [cite_start]3. 模擬實作內容 [cite: 34]
[cite_start]在測試中，我們輸入了 10000,000 和 1000,000 個完全倒序的整數。 [cite: 35] [cite_start]因為平均時間複雜度為 O(N log N)，所以當要排序的數量差 10 倍時，所花的時間大約只會增加 11 到 13 倍左右，而非 100 倍。 [cite: 35] [cite_start]在面對巨量資料時，其執行效率擁有絕對的優勢，幾乎能瞬間完成運算。 [cite: 35]

---

## [cite_start]五、 堆積排序法 (Heap Sort) [cite: 36]

### [cite_start]1. 簡述原理 [cite: 37]
[cite_start]堆積排序法是利用「堆積 (Heap)」這種樹狀資料結構來進行排序。 [cite: 38] [cite_start]首先會將未排序的數列轉換成「最大堆積 (Max-Heap)」，此時陣列的最大值會位於根節點。 [cite: 38] [cite_start]接著將根節點與數列最後一個元素交換（將最大值固定在尾端），並將剩餘元素重新調整為最大堆積。 [cite: 38] [cite_start]重複此過程直到所有元素皆排序完成。 [cite: 38]

### [cite_start]2. 複雜度分析 [cite: 39]
* [cite_start]**最佳時間複雜度**：O(N log N) [cite: 40]
* [cite_start]**最壞 / 平均時間複雜度**：O(N log N) [cite: 41]

### [cite_start]3. 模擬實作內容 [cite: 42]
[cite_start]在測試中，我們輸入了 100,000 和 10,000 個完全倒序的整數。 [cite: 43] [cite_start]與合併排序相似，因為平均時間複雜度被嚴格保證在 O(N log N)，所以當要排序的數量差 10 倍時，所花的時間同樣大約只增加 11 到 13 倍左右。 [cite: 43] [cite_start]不僅速度極快，且不需像合併排序那樣耗費額外的記憶體空間。 [cite: 43]

---

## [cite_start]六、 綜合比較 [cite: 44]

[cite_start]根據我們先前的程式模擬實作與資料量倍增測試，可以得出以下三個核心結論： [cite: 45]

### [cite_start]1. O(N^2) 與 O(N log N) 的巨大效能鴻溝 [cite: 46]
[cite_start]當測試資料量從 1 萬增加到 10 萬（增長 10 倍）時，氣泡、選擇、插入這類 O(N^2) 演算法的執行時間暴增了約 100 倍。 [cite: 47] [cite_start]然而，當資料量從 100 萬筆增加到 1000 萬筆（同樣增長 10 倍）時，合併與堆積這類 O(N log N) 演算法的執行時間僅增加了約 11.5 到 13 倍。 [cite: 48] [cite_start]這在實務上證明了，面對巨量資料時，選擇時間複雜度較低的演算法是唯一的解決方案，硬體的提升無法彌補演算法層級的缺陷。 [cite: 48]

### [cite_start]2. 空間與時間的權衡 [cite: 49]
[cite_start]在 O(N log N) 的頂級演算法中，合併排序與堆積排序展現了不同的設計哲學。 [cite: 50] [cite_start]合併排序採用「空間換取時間與穩定性」的策略，它在執行過程中需要動態配置與原陣列等大（O(N)）的暫存空間；而堆積排序則是極致的「原地排序 (In-place)」，空間複雜度僅需 O(1)，即使處理一千萬筆資料，也不會佔用額外的記憶體負擔，但它輸在對 CPU 硬體架構不友善，CPU 必須不斷停下來等待主記憶體傳送資料，導致實際花費時間更長。 [cite: 51]

### [cite_start]3. 資料初始狀態的影響 [cite: 52]
[cite_start]在最佳情況（資料已經排序好）下，氣泡排序與插入排序可以提早結束迴圈，將時間複雜度降至 O(N)。 [cite: 53] [cite_start]然而，選擇排序無論資料多麼整齊，都必須乖乖執行完整掃描，最佳與最壞時間皆為 O(N^2)。 [cite: 53] [cite_start]因此，如果已知系統中的資料有很大概率是「部分排序」的狀態，插入排序會是 O(N^2) 級別中的最佳選擇。 [cite: 53]