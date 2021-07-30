# Bài 1: Mệnh đề và vị từ

## I. Mệnh đề

### Khái niệm

Trong logic toán học, **mệnh đề** hay đầy đủ là **mệnh đề logic** là một khái niệm nguyên thủy, không định nghĩa.

### Thuộc tính

Mỗi mệnh đề có đúng một trong hay giá trị **1** hoặc **0** tương ứng với giá trị chân lý là **đúng** hoặc **sai**.

*Ví dụ:*

- `Paris là thủ đô của nước Nhật` là một mệnh đề vì nó nhận giá trị chân lý là **sai**.

- `Bây giờ là mấy giờ?` không phải là mệnh đề vì nó không mang giá trị chân lý.

### Ký hiệu

Người ta thường dùng các chữ cái **a, b, c, d,...** làm kí hiệu cho các mệnh đề.

Nếu mệnh đề a có giá trị chân lý là **1** thì ta kí hiệu **G(a) = 1**. *Ngược lại*, **G(a) = 0**.

*Ví dụ:*

- a = `Paris là thủ đô của Nhật Bản` hoặc

- a: `Paris là thủ đô của Nhật Bản`

Ở đây do mệnh đề a **sai** nên ta có **G(a)= 0**

### Các phép toán logic cơ bản

#### Phép phủ định

Phủ định của mệnh đề **a** là một mệnh đề, ký hiệu $\overline{a}$ và có giá trị chân lý ngược lại với giá trị chân lý của **a**

| a   | $\overline{a}$ |
|:---:|:--------------:|
| 1   | 0              |
| 0   | 1              |

*Ví dụ:*

Nếu a: "Hôm nay trời mưa"

$\rightarrow\overline{a}$ = "Hôm nay trời không mưa"

#### Phép hội

Hội của hai mệnh đề a và b là một mệnh đề, đọc là a và b, kí hiệu a Λ b. Đúng trong trường hợp cả a và b đúng và sai trong các trường hợp còn lại.

| a   | b   | a Λ b |
|:---:|:---:|:-----:|
| 0   | 0   | 0     |
| 0   | 1   | 0     |
| 1   | 0   | 0     |
| 1   | 1   | 1     |

*Ví dụ:*

a: "5 là số nguyên tố"

b: "rắn là một loài bò"

$\rightarrow$ a Λ b có giá trị là sai vì b sai.❌

![](https://raw.githubusercontent.com/thangved/images/main/2021/07/30-14-02-05-images.jpg)

#### Phép tuyển

Tuyển của hai mệnh đề a và b là một mệnh đề, đọc là a hoặc b, ký hiệu là a ν b, sai khi cả a và b đều sai và đúng trong các trường hợp còn lại.

| a   | b   | a ν b |
|:---:|:---:|:-----:|
| 0   | 0   | 0     |
| 0   | 1   | 1     |
| 1   | 0   | 1     |
| 1   | 1   | 1     |

*Ví dụ:*

a: "5 là số nguyên tố"

b: "rắn là một loài bò"

$\rightarrow$ a Λ b có giá trị là đúng vì a đúng. ✔️

#### Phép kéo theo

*a kéo theo b* là một mệnh đề, được hiểu là *nếu a thì b*, chỉ sai khi a đúng và b sai và đúng trong các trường hợp còn lại.

| a   | b   | a$\rightarrow$b |
|:---:|:---:|:---------------:|
| 0   | 0   | 1               |
| 0   | 1   | 1               |
| 1   | 0   | 0               |
| 1   | 1   | 1               |

#### Phép tương đương

*a tương đương b* là một mệnh đề, kí hiệu là $a\leftrightarrow b$ nếu cả hai mệnh đề a và b cùng đúng hoặc cùng sai.

<img title="" src="https://raw.githubusercontent.com/thangved/images/main/2021/07/30-14-07-07-bekphnqftcb41-1.jpg" alt="bekphnqftcb41-1.jpg" width="657">

### Một số công thức

#### Phủ định của phủ định

$\overline{\overline{a}}=a$

#### Luật De Morgan

$\overline{a\land b} = \overline{a}\vee\overline{b}$

$\overline{a\vee b} = \overline{a}\land\overline{b}$

#### Tính chất kết hợp

$(a\land b)\land c = a\land(b\land c)$

$(a\vee b)\vee c = a\vee(b\vee c)$
