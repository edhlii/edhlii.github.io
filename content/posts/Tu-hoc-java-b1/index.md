---
date: '2025-10-19T10:56:53+07:00'
draft: false
title: 'Java Buổi 1: Tổng quan về Java, Syntax cơ bản.'
cover:
  image: 'image.png'

---

Chào mina-san!  
Lại là mình đây. Gần đây CLB mình bắt đầu dạy khoá **Java Core**. Tức là dạy về Java và tư duy OOP cơ bản ấy. Nhân cơ hội này mình tranh thủ up các tài liệu mà mình làm lên blog luôn. Để chia sẻ cho mọi người, cũng như để sau này mình xem lại cho tiện 😊.

- [I. Ngôn ngữ Java là gì](#i-ngôn-ngữ-java-là-gì)
- [II. Lý do ra đời của Java](#ii-lý-do-ra-đời-của-java)
- [III. Cách Java hoạt động](#iii-cách-java-hoạt-động)
- [IV. Cấu trúc một chương trình Java](#iv-cấu-trúc-một-chương-trình-java)
- [V. Package là gì?](#v-package-là-gì)
  - [Khai báo package](#khai-báo-package)
  - [Sử dụng package](#sử-dụng-package)
- [VI. Syntax cơ bản](#vi-syntax-cơ-bản)
  - [Khai báo biến nguyên thuỷ](#khai-báo-biến-nguyên-thuỷ)
  - [Vòng lặp](#vòng-lặp)
  - [Lệnh rẽ nhánh](#lệnh-rẽ-nhánh)
  - [Mảng](#mảng)
- [VII. Tổng quan về Class và Object](#vii-tổng-quan-về-class-và-object)
  - [Class và Object](#class-và-object)
  - [Từ khoá this](#từ-khoá-this)
  - [Constructor](#constructor)
  - [Access Modifier](#access-modifier)
  - [Getter, Setter](#getter-setter)
  - [Từ khoá Static](#từ-khoá-static)
- [Lời cuối](#lời-cuối)


## I. Ngôn ngữ Java là gì
Java là một ngôn ngữ lập trình **hướng đối tượng** (Object Oriented Programming -OOP), đa nền tảng. Được **Sun Microsystems** (nay thuộc **Oracle**) phát triển vào năm 1995.  

Nó được thiết kế với khẩu hiệu nổi tiếng:
`Write Once, Run Anywhere`  

Chương trình Java có thể chạy trên mọi hệ điều hành mà không cần sửa đổi mã nguồn - miễn là hệ thống đó có **Java Virtual Machine (JVM)**
## II. Lý do ra đời của Java
Vào đầu những năm 1990, nhóm nghiên cứu của Sun Microsystems muốn tạo ra một ngôn ngữ:
- Có thể chạy trên nhiều thiết bị khác nhau, từ máy tính đến TV, đầu DVD, hoặc thiết bị nhúng.
- An toàn và ổn định hơn C/C++, tránh các lỗi như tràn bộ nhớ hay con trỏ sai.
- Có thể phát triển ứng dụng mạng (Internet) dễ dàng.
- Đơn giản, hướng đối tượng, và dễ bảo trì.
Khi Internet bùng nổ, Java trở thành công cụ lý tưởng để viết ứng dụng web, ứng dụng doanh nghiệp, và sau này là ứng dụng di động (Android).
## III. Cách Java hoạt động
Đầu tiên, ta hãy xét mã nguồn của một chương trình Java cơ bản, tên file là `Hello.java`
```java
public class Hello{
  public static void main(String[] args){
    System.out.println("Hello ProPTIT");
  }
}
```
Tiếp theo, ta biên dịch (compile) chương trình này thành **bytecode**. Output sẽ là file có tên `Heloo.class`.
```bash
javac Hello.java
```
**Lưu ý:** Khác với C/C++, Java compile chương trình thành bytecode, đây không phải mã máy thực, mà là mã được thiết kế cho **JVM**.

Để chạy chương trình, ta sử dụng lệnh:
```bash
java Hello
```
-> Lúc này:
1. **JVM** đọc file `Hello.class`
2. **JVM** kiểm tra bảo mật và chuyển bytecode thành mã máy phù hợp với hệ thống đang chạy (qua **JIT- Just In Time Compiler**)
3. Chương trình được thực thi trên CPU thật
   
Nhờ có cơ chế **JVM** và **JIT** này, nên Java mới có thể chạy trên bất kỳ hệ điều hành nào, chỉ cần cài **JVM** tương ứng.

## IV. Cấu trúc một chương trình Java
Một chương trình Java luôn có ít nhất một class, và hàm `main()` là điểm bắt đầu khi chạy.
Hãy nhìn lại ví dụ lúc nãy:
```java
public class Hello{
  public static void main(String[] args){
    System.out.println("Hello ProPTIT");
  }
}
```

Giải thích từng thành phần:
- `public class Hello`: Khai báo một class tên là Hello. Trong Java, mọi thứ phải nằm trên một class.
- `{ ... }`: Phần thân của class, chứa các **phương thức (method)** và **biến (variable)**.
- `public static void main(String[] args)`: Đây là hàm chính - nơi chương trình bắt đầu chạy
- `System.out.println("...");`: Lệnh in ra màn hình trong Java

## V. Package là gì?
Trong Java, **package** là một cơ chế để tổ chức và quản lý các class, interface, và các thành phần khác thành các nhóm có liên quan với nhau. <br>
### Khai báo package
```java
package ten_package;

public class MyClass {
    // code 
}
```
### Sử dụng package
```java
import ten_package;
```

## VI. Syntax cơ bản
### Khai báo biến nguyên thuỷ
Các kiểu nguyên thuỷ:
- **byte**, **short**, **int**, **long**
- **float**, **double**
- **char**
- **boolean**

Ví dụ
```java
int th = 36;
```
### Vòng lặp
**for:**
```java
for (int i=1; i<=10; ++i){
  System.out.print(i + " ");
}
```
**while**
```java
int i=0;
while(true){
  ++i;
  System.out.print(i + " ");
}
```

### Lệnh rẽ nhánh
**if, else if, else:**
```java
if(<đk>){
  // code 1
} else if(<đk>){
  // code 2
} else{
  // code 3
}
```
**switch-case:**
```java
switch(exp){
  case VALUE:
    // code
    break;
  default:
    //code
}
```
### Mảng
**Khai báo**
Cần khai báo thư viện Array mới sử dụng được.
```java
import java.util.Arrays;
```

Khai báo một array.
```java
int[] a = new int[5]; // Khai báo mảng số nguyên a gồm 5 phần tử
int[] b = {3, 6, 5}; // Khai báo mảng số nguyên b với các phần tử cho trước
```

**Có thể duyệt mảng bằng for-each như C++**

```java
for(int x:a){
  // code
}
```

## VII. Tổng quan về Class và Object
### Class và Object
- **class**: Chứa thuộc tính và hành vi (hiểu như một khuôn đúc)
- **Object**: Thực thể có thuộc tính và hành vi (được đúc từ class)
```java
public class Book{
  private String title;
  private String author;
  public void setTitle(String title){ ... }
  public void burn(){ ... }
}

Book book = new Book();
book.name = "Giao trinh OOP";
book.burn();
```

### Từ khoá this
**this** là từ khoá đại diện cho object, class hiện tại, dùng để phân biệt biến instance (thuộc về đối tượng) và biến local (khai báo trong method).
```java
public void setTitle(String title){
  this.title = title;
}
```
### Constructor
Hàm dùng để khởi tạo đối tượng, trùng tên class.
```java
public class Book{
  private String title;
  private String author;
  public void setTitle(String title){ ... }
  public void burn(){ ... }
}
```
### Access Modifier
- **public**: Truy cập mọi nơi
- **private**: Chỉ truy cập trong class
- **protected**: Trong package + subclass
- **default (không ghi gì)**: Truy cập trong package

### Getter, Setter
Giúp truy cập các trường private
```java
public void setTitle(String title){
  this.title = title;
} 
public String getTitle(){
  return title;
}
```

### Từ khoá Static
Dùng với biến/phương thức để dùng chung cho tất cả class.

```java
public class Obj{
  public static int count = 0;
  public static void sayHello() { ... }
}
// ...
public class Main{
  public class void main(String[] args){
    Obj.sayHello() // gọi trực tiếp
  }
}
```


## Lời cuối
Đây là bài học thuật đầu tiên mình viết nên tự mình thấy nó còn thiếu sót khá nhiều. Cũng chưa được quá chi tiết. Có lẽ mình sẽ chỉnh sửa lại nội dung trong bài trong tương lai để phù hợp hơn. Cảm ơn mọi người đã đọc nha! ❤️