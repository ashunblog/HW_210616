# School_HW_210616

## 1. Prime Number Checker    

### 零、開發環境
•	開發語言：Python
•	編輯器：Vim

### 一、概述
此程式用於判斷任一自然數是否為質數。
依據題目要求，我們要判斷232-1是否為一質數，即4294967295是否為質數。以下圖片為運行結果:
 
 ![image](https://user-images.githubusercontent.com/52514950/124442757-a27c4300-ddaf-11eb-9289-0e67d934c5f9.png)

程式得出的結果顯示，232-1並非唯一質數，在其中一項可能的狀況下，4294967295可背3整除，商為1431655765。

### 二、原理
質數的定義: 在大於1的自然數中，除了1和該數自身外，無法被其他自然數整除的數。
那麼在質數篩選的過程中，我們就可以先排除所有偶數，因為所有偶數皆可被2整除，篩選工作量直接先減半，接下來只要讓待驗證的自然數作為被除數，與剩下的奇數一一相除，若有找到整除的情況，便可判斷此待驗證的數並非質數，反之則為質數。
接下來是範圍問題。直覺上在驗證所有奇數時要一一驗證直到最靠近待驗證數(N)的奇數，但依照埃拉托斯特尼篩法，事實上我們只需篩選到最靠近√N的奇數即可，篩選效率上再進一步提高。




## 2. Letter Frequency Analyzer

### 零、開發環境
-	開發語言：Python
-	編輯器：Vim

### 一、概述
在凱薩密碼的章節中，提到阿拉伯數學家利用字母頻率分析的方法破解凱薩密碼。在以往沒有計算機的時代，字母統計工作只能由人工進行，太大量的文本要統計起來也相對困難，然而時至今日我們有電腦這項利器，幫助我們去統計文章中的字母出現次數。
本程式的目的即為統計文章中字母出現的次數以及計算其出現頻率，並以圖表及列表的方式呈現結果。
