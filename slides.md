---
# You can also start simply with 'default'
theme: dracula
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
# background: https://cover.sli.dev
# some information about your slides (markdown enabled)
title: 5. 陣列＆字串 
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# take snapshot for each slide in the overview
overviewSnapshots: true
---

# 5. 陣列＆字串 
（使用C）

<style>
.text-align-left{
    text-align: left;
}
.text-align-right{
    text-align: right;
}
</style>


---
layout: center
---

### 為什麼需要陣列？

---
title: 如果要記錄5個整數
---

<h3 style="color:white; max-width: fit-content; margin-inline: auto;padding-top: 10px"> 如果要記錄5個整數：</h3>
<br>
<v-click>
<div class="chart1" style="width:300px;  margin-inline: auto; font-size: 30px">
    <style>
        .chart1 table, 
        .chart1 td, 
        .chart1 tr,
        .chart1 th {
          border: none!important;
          border-collapse: collapse;
          text-align: center;
        }
        /* .chart1 td {
          background:  red
        }
        text-align: center; */
    </style>
    <table><tbody>
      <tr>
        <td>int a1;</td>
      </tr>
      <tr>
        <td>int a2;</td>
      </tr>
      <tr>
        <td>int a3;</td>
      </tr>
      <tr>
        <td>int a4;</td>
      </tr>
      <tr>
        <td>int a5;</td>
      </tr>
    </tbody></table>
</div>
</v-click>

---
title: 如果要記錄10個整數
class: text-center
---

<h3 style="color:white; max-width: fit-content; margin-inline: auto;padding-top: 10px">10個呢？</h3>

<br>
<v-click>
<div class="chart1" style="width:300px;  margin-inline: auto; font-size: 30px">
    <style>
        .chart1 table, 
        .chart1 td, 
        .chart1 tr,
        .chart1 th {
          border: none!important;
          border-collapse: collapse;
        }
    </style>
    <table><tbody>
      <tr>
        <td>int a1;</td>
        <td>int a6;</td>
      </tr>
      <tr>
        <td>int a2;</td>
        <td>int a7;</td>
      </tr>
      <tr>
        <td>int a3;</td>
        <td>int a8;</td>
      </tr>
      <tr>
        <td>int a4;</td>
        <td>int a9;</td>
      </tr>
      <tr>
        <td>int a5;</td>
        <td>int a10;</td>
      </tr>
    </tbody></table>
</div>
</v-click> 

---
title: 如果要記錄200個整數
class: text-center
---

<h3 style="color:white; max-width: fit-content; margin-inline: auto;padding-top: 10px">200個呢？</h3>

<br>
<v-click>
<div class="chart2">
    <style>
        .chart2 table, 
        .chart2 td,
        .chart2 tr,
        .chart2 th {
          border: none!important;
          border-collapse: collapse;
          padding: 0px;
          /* border-spacing: 50px; */
          font-size: 14px;
        }
    </style>
    <table>
    <tbody>
      <tr>
        <td>int a1;</td> <td>int a21;</td> <td>int a41;</td> <td>int a61;</td> <td>int a81;</td> <td>int a101;</td> <td>int a121;</td> <td>int a141;</td> <td>int a161;</td> <td>int a181;</td>
      </tr>
      <tr>
        <td>int a2;</td> <td>int a22;</td> <td>int a42;</td> <td>int a62;</td> <td>int a82;</td> <td>int a102;</td> <td>int a122;</td> <td>int a142;</td> <td>int a162;</td> <td>int a182;</td>
      </tr>
      <tr>
        <td>int a3;</td> <td>int a23;</td> <td>int a43;</td> <td>int a63;</td> <td>int a83;</td> <td>int a103;</td> <td>int a123;</td> <td>int a143;</td> <td>int a163;</td> <td>int a183;</td>
      </tr>
      <tr>
        <td>int a4;</td> <td>int a24;</td> <td>int a44;</td> <td>int a64;</td> <td>int a84;</td> <td>int a104;</td> <td>int a124;</td> <td>int a144;</td> <td>int a164;</td> <td>int a184;</td>
      </tr>
      <tr>
        <td>int a5;</td> <td>int a25;</td> <td>int a45;</td> <td>int a65;</td> <td>int a85;</td> <td>int a105;</td> <td>int a125;</td> <td>int a145;</td> <td>int a165;</td> <td>int a185;</td>
      </tr>
      <tr>
        <td>int a6;</td> <td>int a26;</td> <td>int a46;</td> <td>int a66;</td> <td>int a86;</td> <td>int a106;</td> <td>int a126;</td> <td>int a146;</td> <td>int a166;</td> <td>int a186;</td>
      </tr>
      <tr>
        <td>int a7;</td> <td>int a27;</td> <td>int a47;</td> <td>int a67;</td> <td>int a87;</td> <td>int a107;</td> <td>int a127;</td> <td>int a147;</td> <td>int a167;</td> <td>int a187;</td>
      </tr>
      <tr>
        <td>int a8;</td> <td>int a28;</td> <td>int a48;</td> <td>int a68;</td> <td>int a88;</td> <td>int a108;</td> <td>int a128;</td> <td>int a148;</td> <td>int a168;</td> <td>int a188;</td>
      </tr>
      <tr>
        <td>int a9;</td> <td>int a29;</td> <td>int a49;</td> <td>int a69;</td> <td>int a89;</td> <td>int a109;</td> <td>int a129;</td> <td>int a149;</td> <td>int a169;</td> <td>int a189;</td>
      </tr>
      <tr>
        <td>int a10;</td> <td>int a30;</td> <td>int a50;</td> <td>int a70;</td> <td>int a90;</td> <td>int a110;</td> <td>int a130;</td> <td>int a150;</td> <td>int a170;</td> <td>int a190;</td>
      </tr>
      <tr>
        <td>int a11;</td> <td>int a31;</td> <td>int a51;</td> <td>int a71;</td> <td>int a91;</td> <td>int a111;</td> <td>int a131;</td> <td>int a151;</td> <td>int a171;</td> <td>int a191;</td>
      </tr>
      <tr>
        <td>int a12;</td> <td>int a32;</td> <td>int a52;</td> <td>int a72;</td> <td>int a92;</td> <td>int a112;</td> <td>int a132;</td> <td>int a152;</td> <td>int a172;</td> <td>int a192;</td>
      </tr>
      <tr>
        <td>int a13;</td> <td>int a33;</td> <td>int a53;</td> <td>int a73;</td> <td>int a93;</td> <td>int a113;</td> <td>int a133;</td> <td>int a153;</td> <td>int a173;</td> <td>int a193;</td>
      </tr>
      <tr>
        <td>int a14;</td> <td>int a34;</td> <td>int a54;</td> <td>int a74;</td> <td>int a94;</td> <td>int a114;</td> <td>int a134;</td> <td>int a154;</td> <td>int a174;</td> <td>int a194;</td>
      </tr>
      <tr>
        <td>int a15;</td> <td>int a35;</td> <td>int a55;</td> <td>int a75;</td> <td>int a95;</td> <td>int a115;</td> <td>int a135;</td> <td>int a155;</td> <td>int a175;</td> <td>int a195;</td>
      </tr>
      <tr>
        <td>int a16;</td> <td>int a36;</td> <td>int a56;</td> <td>int a76;</td> <td>int a96;</td> <td>int a116;</td> <td>int a136;</td> <td>int a156;</td> <td>int a176;</td> <td>int a196;</td>
      </tr>
      <tr>
        <td>int a17;</td> <td>int a37;</td> <td>int a57;</td> <td>int a77;</td> <td>int a97;</td> <td>int a117;</td> <td>int a137;</td> <td>int a157;</td> <td>int a177;</td> <td>int a197;</td>
      </tr>
      <tr>
        <td>int a18;</td> <td>int a38;</td> <td>int a58;</td> <td>int a78;</td> <td>int a98;</td> <td>int a118;</td> <td>int a138;</td> <td>int a158;</td> <td>int a178;</td> <td>int a198;</td>
      </tr>
      <tr>
        <td>int a19;</td> <td>int a39;</td> <td>int a59;</td> <td>int a79;</td> <td>int a99;</td> <td>int a119;</td> <td>int a139;</td> <td>int a159;</td> <td>int a179;</td> <td>int a199;</td>
      </tr>
      <tr>
        <td>int a20;</td> <td>int a40;</td> <td>int a60;</td> <td>int a80;</td> <td>int a100;</td> <td>int a120;</td> <td>int a140;</td> <td>int a160;</td> <td>int a180;</td> <td>int a200;</td>
      </tr>
    </tbody></table>
</div>
</v-click>
<v-click>
<div class="absolute inset-0 flex justify-center items-center">
  <div class="text-center leading-tight" style="padding-top:130px">
  <strong><span style="font-size: 155px; color: white;">當然<br>不是</span></strong>
  </div>
</div>
</v-click>

---
title: 所以我們需要陣列
layout: center
---

<div class="grid grid-cols-1 gap-6 ...">
<div class="place-self-center">
  <h4 style="color:white; font-size:38px!important;">所以我們需要</h4>
</div>
  <div class="place-self-center">

<h2 style="color:white;">陣列</h2></div>
</div>

---
layout: center
class: text-3xl space-y
font_adjustment: 1
---

### 何謂陣列？

<br />
<v-click>

**陣列(array)** 是一種用來儲存資料的資料結構

陣列中的每個元素都是<u>相同</u>的資料型態

利用 **索引(index)** 就可以找出對應的元素(element)

</v-click>


---
title: 陣列圖
---

![](https://hackmd.io/_uploads/r1pyO6nAC.png)

- 因此一個長度為5的陣列就有索引為0, 1, 2, 3, 4的五個元素


<div class="text-align-right">
    
<span style="font-size:30px;"><span color="#f00">*</span>陣列的第一個元素是從0開始的</span>
    
</div>

<!-- 
記憶體 \
陣列是一段記憶體空間 -->


---

### 陣列的特性：

<div class="smaller">
<v-clicks>

* **相同類型的元素** \
  所有元素都是相同類型的，例如整數、浮點數、字元等。

* **連續的記憶體空間** \
  陣列的元素在記憶體中是連續存放的。

* **索引訪問** \
  每個元素都有一個唯一的索引，可以使用索引來訪問和修改特定位置的元素。
  <br>
  例如：`arr[3]`, `arr[0]`
  <br>
  <div style="font-size:20px"><span style="color:#f00">*</span>索引值必 > 0</div>

* **固定大小** \
  陣列在創建時需要指定大小，且一旦分配了大小，通常不能動態改變。

</v-clicks>
</div>


---
title: 陣列的宣告
class: text-2xl space-y-5
md: leading-loose
---

<h3 style="font-size: 40px">陣列的宣告：</h3>


<div class="text-align-left smaller">

* 創建一個整數(int)陣列

```c{*}{lines:false, class:'!children:text-0.95rem'}
// 給定數值編譯器自動判斷陣列大小
int integerArray[] = {2,7,6,8,3};

// 創建一個長度5的int陣列，不給定初始值
int integerArray2[5];

// 創建一個長度5的int陣列，給定預設初始值(0)
int integerArray3[5]={};

// 創建一個長度5的int陣列，給定某些初始值，其它為0
int integerArray3[5]={2,3}; // 2,3,0,0,0
    
```

* 創建一個浮點(float/double)陣列
```c{*}{lines:false, class:'!children:text-0.95rem'}
float arr1[] = {2.3, 5.4, 9.3, 8.03};
double arr2[] = {8.3, 2.7, 3.6};
```

</div>

---
title: Array 範例1(0)
transition: fade
---

Array 範例1

```c {*}{lines:true, class:'!children:text-1.1rem'}
#include <stdio.h>
int main(){
    int arr[5] = {2,4,7,8,3};
    for (int i=0; i<5; i++){
        printf("%d ", arr[i]);
    }
    printf("\n");
    return 0;
}
```

---
title: Array 範例1(1)
---

Array 範例1

```c {*}{lines:true, class:'!children:text-1.1rem'}
#include <stdio.h>
int main(){
    int arr[5] = {2,4,7,8,3};
    for (int i=0; i<5; i++){
        printf("%d ", arr[i]);
    }
    printf("\n");
    return 0;
}
```

印出：

```plaintext {*}{lines:false, class:'!children:text-1.1rem'}
2 4 7 8 3
```

---
title: Array 範例2.1(0)
transition: fade
---

Array 範例2.1

<div class="flex flex-row" style="width:870px;">
  <div class="basis-65/100" style="padding: 0px 50px 0px 10px; ">
```c{*}{lines:true, class:'!children:text-1.05rem'}
#include <stdio.h>
int main(){
    int arr[4];
    for (int i=0; i<4; i++){
        scanf("%d", &arr[i]);
    }
    
    int sum = 0;
    for (int i=0; i<4; i++){
        sum += arr[i];
    }

    printf("sum = %d\n", sum);
    printf("avg = %d\n", sum/4);
    return 0;
}
```
  </div>
  <div class="basis-35/100">
  <p>輸入：</p>

```plaintext {*}{lines:false, class:'!children:text-1.1rem'}
5 13 4 9
```

<br>

  </div>
</div>

---
title: Array 範例2.1(1)
---

Array 範例2.1

<div class="flex flex-row" style="width:870px;">
  <div class="basis-65/100" style="padding: 0px 50px 0px 10px; ">
```c{*}{lines:true, class:'!children:text-1.05rem'}
#include <stdio.h>
int main(){
    int arr[4];
    for (int i=0; i<4; i++){
        scanf("%d", &arr[i]);
    }
    
    int sum = 0;
    for (int i=0; i<4; i++){
        sum += arr[i];
    }

    printf("sum = %d\n", sum);
    printf("avg = %d\n", sum/4);
    return 0;
}
```
  </div>
  <div class="basis-35/100">
  <p>輸入：</p>

```plaintext {*}{lines:false, class:'!children:text-1.1rem'}
5 13 4 9
```

<br>


<p>輸出：</p>
```plaintext {*}{lines:false, class:'!children:text-1.1rem'}
sum = 31
avg = 7
```

  </div>
</div>

---
title: Array 範例2.2(0)
transition: fade
---

Array 範例2.2

<div class="flex flex-row" style="width:870px;">
  <div class="basis-70/100" style="padding: 0px 50px 0px 10px; ">
```c{*}{lines:true, class:'!children:text-1.05rem'}
#include <stdio.h>
int main(){
    int arr[4];
    for (int i=0; i<4; i++){
        scanf("%d", &arr[i]);
    }
    
    int sum = 0;
    for (int i=0; i<4; i++){
        sum += arr[i];
    }

    printf("sum = %d\n", sum);
    printf("avg = %.2lf\n", (double)sum/4);
    return 0;
}
```
  </div>
  <div class="basis-30/100">
  <p>輸入：</p>

```plaintext {*}{lines:false, class:'!children:text-1.1rem'}
5 13 4 9
```

<br>

  </div>
</div>

---
title: Array 範例2.2(1)
---

Array 範例2.2

<div class="flex flex-row" style="width:870px;">
  <div class="basis-70/100" style="padding: 0px 50px 0px 10px; ">
```c{*}{lines:true, class:'!children:text-1.05rem'}
#include <stdio.h>
int main(){
    int arr[4];
    for (int i=0; i<4; i++){
        scanf("%d", &arr[i]);
    }
    
    int sum = 0;
    for (int i=0; i<4; i++){
        sum += arr[i];
    }

    printf("sum = %d\n", sum);
    printf("avg = %.2lf\n", (double)sum/4);
    return 0;
}
```
  </div>
  <div class="basis-30/100">
  <p>輸入：</p>

```plaintext {*}{lines:false, class:'!children:text-1.1rem'}
5 13 4 9
```

<br>

<p>輸出：</p>
```plaintext {*}{lines:false, class:'!children:text-1.1rem'}
sum = 31
avg = 7.75
```
  </div>
</div>

---
layout: center
---

# 字串

---
title: 字串是什麼？
layout: center
---

<div class="grid grid-cols-1 gap-6 ...">
    <div class="place-self-center">
        <h2>字串是什麼？</h2>
    </div>
    <div class="place-self-center mybody">
        其實字串就是一種字元陣列
    </div>
</div>

---

### 字串的宣告

<div style="padding-top: 45px">
```c{*}{lines:false, class:'!children:text-1.5rem'}
char s[] = {'a', 'p', 'p', 'l', 'e', '\0'};
```

`\0` 是結束字元，代表字串結尾。

<br>

```c{*}{lines:false, class:'!children:text-1.5rem'}
char s[] = "apple";
```

與上面相同效果

</div>

---
title: 字串範例(0)
transition: fade
---

字串範例：

<div class="flex flex-row" style="width:870px;">
    <div class="basis-76/100" style="padding: 0px 50px 0px 10px; ">
```c{*}{lines:false, class:'!children:text-1.2rem'}
#include <stdio.h>
int main(){
    char s1[] = "Hello, World";
    char s2[] = {'H', 'E', 'L', 'L', 'O', '\0'};

    printf("%c %c\n", s1[4], s2[1]);
    printf("%s\n", s1);
    printf("%s\n", s2);

    return 0;
}
```


</div>
</div>

---
title: 字串範例(1)
---

字串範例：

<div class="flex flex-row" style="width:870px;">
    <div class="basis-76/100" style="padding: 0px 50px 0px 10px; ">
```c{*}{lines:false, class:'!children:text-1.2rem'}
#include <stdio.h>
int main(){
    char s1[] = "Hello, World";
    char s2[] = {'H', 'E', 'L', 'L', 'O', '\0'};

    printf("%c %c\n", s1[4], s2[1]);
    printf("%s\n", s1);
    printf("%s\n", s2);

    return 0;
}
```

</div>
    <div class="basis-24/100">
    <p>輸出：</p>

```plaintext{*}{class:'!children:text-1.2rem'}
o E
Hello, World
HELLO
```

</div>
</div>

---
title: 補充：其它字串相關函式
layout: center
---

<div style="width: 400px">

補充：其它字串相關函式


```c{*}{lines:false, class:'!children:text-1.1rem'}
// 使用以下函式需要引入此標頭檔
#include <string.h>
```

<br>

```c{*}{lines:false, class:'!children:text-1.1rem'}
// 將s1之內容複製到s2
strcpy(destination, source);

// 比較字串之字典序
strcmp(s1, s2)

// 將s2的內容加到s1之後
strcat(s1, s2);
```
</div>