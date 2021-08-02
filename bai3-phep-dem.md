# Bài 3: Phép đếm

- *Như các bạn đã biết (hoặc chưa), đếm 🐑 là một bộ môn thể thao thường được chơi khi chúng ta mất ngủ và ai cũng biết nên chúng ta chẳng việc gì phải học trong khóa này cả 🤣.*

- *Mà thay vào đó trong bài này, chúng ta sẽ được tìm hiểu về **các nguyên lý đếm, đại số tổ hợp** và **hệ thức truy hồi**.*

## Các nguyên lý đếm

### Quy tắc cộng

> Giả sử một việc nào đó có 2 phương án thực hiện A và B.
> 
> - Phương án A có $m$ cách thực hiện.
> 
> - Phương án B có $n$ cách thực hiện.
> 
> $\rightarrow$ Tổng số cách để hoàn thành công việc này là $m + n$.

### Quy tắc nhân

> Giả sử một công việc gồm hai bước 1 và 2.
> 
> - Bước 1 có $m$ cách thực hiện.
> 
> - Bước 2 có $n$ cách thực hiện.
> 
> $\rightarrow$ Tổng số cách thực hiện là $mn$.

**Ví dụ**

> Tính số cách để anh thợ điện có thể đi đến nhà cô gái.
> 
> ![li.png](https://raw.githubusercontent.com/thangved/images/main/2021/08/02-13-13-19-li.png)
> 
> *Để đi từ **A** đến **D** ta phải đi từ **A** đến **B**, **B** đến **C** và **C** đến **D**.*
> 
> - Đi từ A đến B có 4 cách.
> 
> - Đi từ B đến C có 2 cách.
> 
> - Đi từ C đến D có 3 cách.
> 
> ---
> 
> $\rightarrow$ có $4*2*3=24$ cách.

## Đại số tổ hợp

### Hoán vị

**Công thức**

> 🔥 Số hoán vị của n phần tử là $n!$ với $n\in Z^{+}$.

**Sử dụng**

> 🖊️ Hoán vị được dùng khi bạn cần sắp xếp n phần tử vào n vị trí và các vị trí có sự phân bệt (sắp xếp).

**Ví dụ**

> Số cách để sắp 5 người vào 5 chỗ ngồi.
> 
> ---
> 
> $5!=120$

### Chỉnh hợp

**Công thức**

>  🔥 Số chỉnh hợp: $A_{n}^{k}={{n!}\over{(n-k)!}}$ với $n,k\in Z^{+},n\geq k$.
> 
> Thấy có vẻ nhiều nhưng thật ra chỉ cần bấm máy 🤣

**Cách bấm máy:**

> *Để tính $A_{5}^{3}$ ta bấm như sau: `3`,`SHIFT`+`nPr`,`5`*
> 
> <img title="" src="https://raw.githubusercontent.com/thangved/images/main/2021/08/02-17-07-07-227014513_200702632014224_2880166419295607917_n.jpg" alt="227014513_200702632014224_2880166419295607917_n.jpg" width="352">

**Sử dụng**

> 🖊️ Ta sử dụng chỉnh hợp khi cần sắp xếp k phần tử vào m vị trí từ n phần tử $(n\geq k)$ và các vị trí có sự phân biệt (sắp xếp).
> 
> - Trường hợp $n=k$ là trường hợp hoán vị.

**Ví dụ**

> Lớp **DI20Z6A1** có 59 thành viên. Cần bầu ra 3 bạn vào BCH, một bạn làm Bí thư, một bạn làm Phó bí thư và một bạn làm Ủy viên. Hỏi có bao nhiêu trường hợp có thể xảy ra.
> 
> ---
> 
> *Số trường hợp có thể xảy ra là:* $A_{59}^{3}=195054$.

### Tổ hợp

**Công thức**

> 🔥 Số tổ hợp: $C_{n}^{k}={{n!}\over{k!(n-k)!}}$ với $n,k\in Z^{+},n\geq k$.
> 
> Cái này cũng **bấm máy nuôn cho ló nhanh.**

**Cách bấm máy**

> Để tính $C_{3}^{5}$ ta bấm máy như sau: `5`, `SHIFT`+`nCr`, `3`.
> 
> <img src="https://raw.githubusercontent.com/thangved/images/main/2021/08/02-17-36-40-225372629_200714898679664_7799667796335471808_n.jpg" title="" alt="225372629_200714898679664_7799667796335471808_n.jpg" width="354">

**Sử dụng**

> 🖊️ Ta sủ dụng tổ hợp khi cần **lựa chọn** k phần tử từ tập b phần tử (không có sự sắp xếp).

**Ví dụ**

> Lớp **DI20Z6A1** tiếp tục có 59 thành viên. Cần cử ra 5 bạn để tham gia lao động. Có bao nhiêu trường hợp xảy ra?
> 
> ---
> 
> *Số trường hợp có thể xảy ra là:* $C_{59}^{5}=5006386$.

### Bài tập tổng hợp

> Lại là lớp **DI20Z6A1** có 59 thành viên trong đó có 6 nữ và những bạn còn lại là nam (hoặc không). Lớp cần bầu ra 5 bạn để làm BCH với điều kiện có ít nhất một bạn nữ.
> 
> ---
> 
> *Đáp án: 2136701*

## Hệ thức truy hồi
