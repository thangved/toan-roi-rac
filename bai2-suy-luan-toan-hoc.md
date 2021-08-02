# Bài 2: Suy luận toán học

## Các quy tắc suy luận

> 🙄 Trước khi bắt đầu, thì đây là những quy tắc đã được chứng minh. Các bạn **không nhất thiết** phải hiểu những công thức này mà chỉ cần áp dụng vào giải các bài tập.
> 
> Còn muốn hiểu thì các bạn có thể tự phân tích nó, cũng không khó lắm đâu.
> 
> <img title="" src="https://raw.githubusercontent.com/thangved/images/main/2021/08/01-18-07-56-t%E1%BA%A3ixu%E1%BB%91ng.jpg" alt="tảixuống.jpg" width="138" data-align="center">

> | Quy tắc                                                | Hằng đúng                                                            | Tên                    |
> |:------------------------------------------------------:|:--------------------------------------------------------------------:|:----------------------:|
> | $P\over{P\vee Q}$                                      | $P\rightarrow (P\vee Q)$                                             | Cộng                   |
> | ${P\land Q}\over{P}$                                   | $P\land Q\rightarrow P$                                              | Rút gọn                |
> | ${P,P\rightarrow Q}\over{Q}$                           | $(P\land(P\rightarrow Q))\rightarrow Q$                              | Khẳng định             |
> | ${\overline{Q},P\rightarrow{Q}\over{\overline{P}}}$    | $(\overline{Q}\land (P\rightarrow Q)\rightarrow\overline{P})$        | Phủ định               |
> | ${P\rightarrow Q,Q\rightarrow R}\over{P\rightarrow R}$ | $((P\rightarrow Q)\land(Q\rightarrow R))\rightarrow(P\rightarrow R)$ | Tam đoạn luận giả định |
> | ${\overline{P},(P\vee Q)}\over{Q}$                     | $(\overline{P}\land(P\vee Q))\rightarrow Q$                          | Tam đoạn luận tuyển    |

## Các phương pháp chứng minh

> ⚠️ Trên lớp thì các bạn sẽ có thể được học nhiều phương pháp chứng minh, nhưng lúc thi thì thường giảng viên chỉ cho phương pháp **chứng minh quy nạp** nên mình chỉ đề cập đến phương pháp này.

### Quy nạp

#### Khái niệm

> 🙃 Làm gì có khái niệm.
> 
> Mà thay vào đó, chúng ta hãy xem các bước chứng minh, bao đơn giản (còn không thì thôi 🙄).

#### Các bước chứng minh

> Chứng minh $P(n)$ luôn đúng với $n\geq {n}_{0}$

> **Bước 1:** Kiểm chứng $P({n}_{0})$
> 
> - Nếu $P({n}_{0})$ **sai**: thì kết luận luôn là $P(n)$ sai.
> 
> - Nếu $P({n}_{0})$ **đúng** thì sang bước 2 🤨.

> **Bước 2:** Giả sử $P(k)$ đúng, bạn chỉ cần chứng minh $P(k+1)$ đúng là được 🐧
> 
> - Nếu $P(k + 1)$ **sai**: thì kết luận luôn là $P(n)$ sai.
> 
> - Nếu $P(k + 1)$ **đúng**: thì kết luận luôn là $P(n)$ đúng.

<img title="" src="https://raw.githubusercontent.com/thangved/images/main/2021/08/02-08-49-59-giphy.webp" alt="giphy.webp" data-align="center" width="160">

**Các bạn có cảm thấy nó dễ hiểu không? Chắc chắn là 😾 hiểu. Vậy thì hãy làm thử một ví dụ sau đây nhé!**

**Ví dụ**

> Cho $n \geq 1$. Chứng minh rằng:
> 
> $\mathrm{P}(\mathrm{n}): \sum_{\mathrm{i}=1}^{\mathrm{n}} \mathrm{i}=1+2+3+\ldots+\mathrm{n}=\frac{\mathrm{n}(\mathrm{n}+1)}{2}$

**Bước 1:** Kiểm chứng $P({n}_{0})$: Thay $n=1$ vào 2 vế

> - VT: $\sum_{i=1}^{n}i = 1$
> 
> - VP: ${{n(n + 1)\over{2}}} = {{1(1+1)}\over{2}} = 1$
> 
> $\rightarrow$ VT = VP
> 
> $\rightarrow$ P(1) đúng.

**Bước 2:** Giả sử $P(k)$ *đúng*

> Ta có:
> 
> ${\sum_{i=1}^{k}i} = {{k(k+1)}\over{2}}$
> 
> *Lúc này,* ta chỉ cần chứng minh $P(k+1)$ đúng, đồng nghĩa với việc:
> 
> $\sum_{i=1}^{k+1}i = {{(k+1)(k+1+1)}\over{2}}$

**Chứng minh:**

> Ta có:
> 
> ${\sum_{i=1}^{k}i} = {{k(k+1)}\over{2}}$
> 
> $\rightarrow{\sum_{i=1}^{k}i+k+1}={{k(k+1)}\over{2}}+k+1$
> 
> $\leftrightarrow\sum_{i=1}^{k+1}={{k(k+1)+2(k+1)}\over{2}}$
> 
> $\leftrightarrow\sum_{i=1}^{k+1}={{(k+1)(k+2)}\over{2}}$ *(điều phải chứng minh)*
> 
> $\rightarrow P(k+1)$ **đúng**

***Vậy: P(n) đúng ✔️***

#### Bài tập 🖊️

> Với $n\geq 1$ và n là số nguyên, hãy chứng minh:
> 
> $\sum_{i=1}^{n}(2 i-1)=1+3+5+\ldots .+(2 n-1)=n^{2}$
