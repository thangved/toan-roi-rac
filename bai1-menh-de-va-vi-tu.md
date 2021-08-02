# Bài 1: Mệnh đề và vị từ

## I. Mệnh đề

### Khái niệm

> 🔥 Trong logic toán học, **mệnh đề** hay đầy đủ là **mệnh đề logic** là một khái niệm nguyên thủy, không định nghĩa.

### Thuộc tính

> Mỗi mệnh đề có đúng một trong hay giá trị **1** hoặc **0** tương ứng với giá trị chân lý là **đúng ✔️** hoặc **sai ❌**.

*Ví dụ:*

- `🙂 Paris là thủ đô của nước Nhật` là một mệnh đề vì nó nhận giá trị chân lý là **sai**.

- `⏱️ Bây giờ là mấy giờ?` không phải là mệnh đề vì nó không mang giá trị chân lý.

### Ký hiệu

>  Người ta thường dùng các chữ cái **$P,Q,R,S$,...** làm kí hiệu cho các mệnh đề. Nếu mệnh đề $P$ có giá trị chân lý là **1** thì ta kí hiệu $P=1$. *Ngược lại*, $P=0$.

*Ví dụ:*

- $P$ = `Paris là thủ đô của Nhật Bản` hoặc

- $P$: `Paris là thủ đô của Nhật Bản`

Ở đây do mệnh đề a **sai** nên ta có $P=0$

### Các phép toán logic cơ bản

#### Phép phủ định

> Phủ định của mệnh đề **a** là một mệnh đề, ký hiệu \overline{a} và có giá trị chân lý ngược lại với giá trị chân lý của **a**
> 
> | $P$ | $\overline{P}$ |
> |:---:|:--------------:|
> | 0   | 1              |
> | 1   | 0              |

*Ví dụ:*

Nếu $P$: "Hôm nay trời mưa"

$\rightarrow \overline{P}$ = "Hôm nay trời không mưa"

#### Phép hội

> 🔥 Hội của **hai mệnh đề** a và b là một mệnh đề, đọc là  $P và Q$, kí hiệu $P\land Q$. Đúng trong trường hợp cả a và b đúng và sai trong các trường hợp còn lại.
> 
> | $P$ | $Q$ | $P\land Q$ |
> |:---:|:---:|:----------:|
> | 0   | 0   | 0          |
> | 0   | 1   | 0          |
> | 1   | 0   | 0          |
> | 1   | 1   | 1          |

> 💡 Mẹo: Các bạn có thể hiểu nó như phép nhân dị đóa. 1 nhân 1 thì bằng 1, còn 0 nhân số mấy cũng bằng 0.

> *Ví dụ:*
> 
> $P$: "5 là số nguyên tố"
> 
> $Q$: "rắn là một loài bò 🐮"
> 
> *Giải:*
> 
> Ta có:
> 
> - $P $**đúng** $\rightarrow P = 1$
> 
> - $Q$ **sai** $\rightarrow Q=0$
> 
> - $P*Q=1*0=0$
> 
> - $\rightarrow P\land Q$ có giá trị là sai vì $Q$ sai.❌
> 
> <img src="https://raw.githubusercontent.com/thangved/images/main/2021/07/30-14-02-05-images.jpg" title="" alt="" width="253">

#### Phép tuyển

> 🔥 Tuyển của hai mệnh đề $P$ và $Q$ là một mệnh đề, đọc là $P$ hoặc $Q$, ký hiệu là $P\vee Q$, sai khi cả $P$ và $Q$ đều sai và đúng trong các trường hợp còn lại.
> 
> | $P$ | $Q$ | $P\vee Q$ |
> |:---:|:---:|:---------:|
> | 0   | 0   | 0         |
> | 0   | 1   | 1         |
> | 1   | 0   | 1         |
> | 1   | 1   | 1         |

> *Ví dụ:*
> 
> - $P$: "5 là số nguyên tố"
> 
> - $Q$: "rắn là một loài bò🐮"
> 
> - $P\vee Q$ có giá trị là đúng vì $P$ đúng. ✔️

#### Phép kéo theo

> 🔥 *$P$kéo theo $Q$* là một mệnh đề, được hiểu là *nếu $P$ thì $Q$*, chỉ sai khi $P$ đúng và $Q$ sai và đúng trong các trường hợp còn lại.
> 
> | $P$ | $Q$ | $P\rightarrow Q$ |
> |:---:|:---:|:----------------:|
> | 0   | 0   | 1                |
> | 0   | 1   | 1                |
> | 1   | 0   | 0                |
> | 1   | 1   | 1                |

#### Phép tương đương

> 🔥 *$P$ tương đương $Q$* là một mệnh đề, kí hiệu là $P\leftrightarrow Q$ nếu cả hai mệnh đề $P$ và $Q$ cùng đúng hoặc cùng sai.

<img title="" src="https://raw.githubusercontent.com/thangved/images/main/2021/07/30-14-07-07-bekphnqftcb41-1.jpg" alt="bekphnqftcb41-1.jpg" width="277" data-align="center">

### Một số công thức

> |                       | Công thức                                          | Giải thích                                                                         |
> |:---------------------:|:--------------------------------------------------:|:----------------------------------------------------------------------------------:|
> | Phủ định của phủ định | $\overline{\overline{P}}=P$                        | Giống như - (-1) thì bằng 1, hỏng cần giải thích hihi 🤣                           |
> | Luật De Morgan        | $\overline{P\land Q}=\overline{P}\vee\overline{Q}$ |                                                                                    |
> |                       | $\overline{P\vee Q}=\overline{P}\land\overline{Q}$ |                                                                                    |
> | Tính chất kết hợp     | $(P\land Q)\land R = P\land(Q\land R)$             |                                                                                    |
> |                       | $(P\vee Q)\vee R=P\vee(Q\vee R)$                   |                                                                                    |
> | Tính chất giao hoán   | $P\land Q=Q\land P$                                | $P*Q=Q*P$                                                                          |
> |                       | $P\vee Q=Q\vee P$                                  | $P + Q=Q+P$                                                                        |
> |                       | $P\leftrightarrow Q=Q\leftrightarrow P$            | Hiểu đơn giản thì so sánh bằng a với b hay b với a thì đều cho kết quả như nhau 🙄 |
> | Tính chất phân phối   | $P\land (Q\vee R)=(P\land Q)\vee(P\land R)$        |                                                                                    |
> |                       | $P\vee(Q\land R)=(P\vee Q)\land(P\vee R)$          |                                                                                    |

> 😛 Các bạn không nhất thiết phải học thuộc hết các công thức này. Các bạn có thể nhớ được nó trong quá trình làm bài tập.
> 
> <img title="" src="https://raw.githubusercontent.com/thangved/images/main/2021/07/31-09-35-33-giphy%20(1).webp" alt="giphy (1).webp" width="126">

## Vị từ

> 🔥 Một vị từ là một khẳng định $P(x,y,...)$ trong đó có chứa một số biến x, y, ... lấy giá trị trong tập hợp $A,B,...$ cho trước, sao cho:
> 
> - Bản thân $P(x,y,...)$ **không phải** là mệnh đề.
> 
> - Nếu thay $x,y,...$ bằng những **giá trị cụ thể** thuộc tập hợp $A,B,...$ cho trước ta sẽ được một mệnh đề $P(x,y,...)$. Các biến $x,y,...$ được gọi là các biến tự do của vị từ.

> *Ví dụ:* $P(n)=$ {n là chẵn}
> 
> - $n = 2\rightarrow P(n)=1$
> 
> - $n=5\rightarrow P(n)=0$

### Công thức logic

*Tương tự với mệnh đề 🙂*
