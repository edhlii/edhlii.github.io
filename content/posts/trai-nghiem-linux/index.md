---
date: "2025-02-21T08:25:26+07:00"
title: "Trải nghiệm dùng Linux của mình (Arch btw)"
draft: false
cover:
  image: "arch.png"
---

Chào mọi người!

Không dài dòng, thì như cái tiêu đề, mình là một người dùng Linux fulltime (Arch btw). Mình viết bài này để chia sẻ trải nghiệm của mình, để các bạn có thể tham khảo và cân nhắc xem nên chuyển qua Linux không. Bây giờ vào nội dung chính nha 😊

# Tại sao dùng Linux 🐧

Quay lại hồi cấp 3 của mình. Lúc đó mình chỉ có con laptop cùi cùi, lướt web còn lag (mấy og đừng có bảo tôi coi cái gì vớ vẩn nhá 😮). Lí do vì Windows rất là **bloat**. Nên mình quyết định thử chuyển qua Linux dùng, vì mình nghe nói Linux nhẹ hơn Windows rất nhiều. Sau đó thì dùng quen nên dùng tới bây giờ luôn lmao 🤣.

Thêm nữa là linux hoàn toàn **free** và **mã nguồn mở**, bạn sẽ không phải tốn một xu khi cài đặt linux. Và hầu hết các phần mềm trên linux cũng như vậy, nên nếu bạn không có dư tiền thì nên cân nhắc linux nhé. Hoặc các bạn có thể tà đạo dùng Windows cờ rắc ...khụ...khụ.

Nếu bạn theo chuyên ngành cntt nói chung thì nên tìm hiểu Linux nhé. Hệ điều hành này được ứng dụng rất nhiều đấy. Theo trải nghiệm cá nhân mình thì việc set-up project trên linux tiện hơn windows nhiều 🚀. Bạn gõ vài lệnh trên `CLI` và mọi thứ đã sẵn sàng để bạn bắt tay vào code. Còn trên Windows thì bạn sẽ phải đánh nhau với cái hệ điều hành, fix cả đống các lỗi mà không liên quan đến dự án bạn đang làm, sau đó mới bắt tay vào code được. Đây là trải nghiệm của mình với thư viện raylib, C++ so sánh giữa Win và Linux đó 😇.

```
Cấu hình laptop cũ của mình:
- CPU: Intel Celeron N3060
- GPU: Intergrated
- Ram: 4GB
- HDD: 500GB
```

# Linux Distro đầu tiên🐦

Mình đã thử nghiệm với **Lubuntu**. Cái này là một distro giống ubuntu nhưng mà nhẹ hơn nhiều. Dùng LXQt nếu mình nhớ không nhầm (ae tra google cái này nha🤣). Lúc đó mình cài Lubuntu dual boot với Windows.

![Anh minh hoa lubuntu](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdebugpointnews.com%2Fwp-content%2Fuploads%2F2022%2F08%2FLubuntu-22.04-with-LXQt-1.1.0.jpg&f=1&nofb=1&ipt=9330122b5e4bdbad72916ee46e7a71d907a0b04e473deca2dc64c9e89d5ab509&ipo=images "lubuntu") _Lubuntu nhìn như thế này._

Mình dùng thấy nhanh hơn hẳn Windows 🚀. Bình thường lúc mới khởi động Windows ăn hơn 50% RAM, giờ qua dùng cái này thấy máy chạy nhàn hơn nhiều.

Lúc này mình vẫn dùng linux như windows thôi. Mình bắt đầu tập tành dùng dòng lệnh `CLI` các thứ các thứ.

Thực sự là dùng CLI là một cái gì đấy rất khó tả. Cảm giác lướt ngón tay trên **terminal** rất gây nghiện. Với CLI của linux bạn có thể làm gần như mọi thứ. Một điều mình rất thích của linux đó là tải phần mềm (thường gọi là package) bằng dòng lệnh luôn.
Ví dụ cho việc tải firefox:

```
sudo apt install firefox
```

Tất nhiên không thể thiếu các lệnh cơ bản, như `cd`, `mkdir`, `rm`, ...

Và tất nhiên là lệnh `neofetch` nữa =)).

Quên chưa nói các bạn, trước khi dùng nó một cách _bình thường_ thì mình phải set-up kha khá. Phải tự mày mò tìm cách cài driver card màn hình tích hợp, bộ gõ tiếng việt, rồi khi cài không được thì phải tra google lỗi đến mệt nghỉ luôn 🤣. Nhiều khi mình làm theo y hệt hướng dẫn mà nó vẫn lỗi, ảo vê xê lờ. Sau khi vật lộn đánh nhau với cái máy tính thì nó đã hoạt động bình thường 😅. Tuy mệt nhưng mà việc mày mò vọc vạch như vậy mình thấy khá vui, cảm thấy một việc rất đơn giản thôi, nhưng làm nó hoạt động được trên linux mình tự nhiên thấy mình vjppromax thực sự 🚀.

Tuy nhiên lúc đó mình sắp thi HSG tin học, mà khổ cái tỉnh mình vẫn dùng CD để lưu bài làm. Phải dùng phần mềm gì trên Windows để burn CD ấy, mình quên tên cmnr🤣. Đại khái là không dùng linux đi thi được. Thế là mình quay lại dùng Windows để cho quen tay.

Thời gian trôi nhanh như chó chạy ngoài đồng. Cuối cùng thì mình đã đạt kết quả khá ổn trong kì thi HSG tỉnh. Cụ thể thì mình đạt giải Ba. Và bố mẹ đã tài trợ tiền lên đời máy cho mình kkk 🤑. Nên mình đã lên ngay một quả distro khác 😋.

# Linux có gì hay 🤨

Lần này mình xin mua máy bàn, vì nó có hiệu năng trên giá thành tốt hơn laptop.
Tiền mình được không quá nhiều, nên mình phải suy nghĩ kĩ để mua một bộ hợp lí (cụ thể thì mình có 5 củ khoai 🥔)

Đen cái lúc đó đúng lúc đang bão giá card đồ họa nữa, thành ra mình mua đc bộ vẫn tương đối cùi. Nhưng mình thấy nó đủ đáp ứng nhu cầu của mình, và tới giờ mình vẫn đang dùng bộ này.

```
Cấu hình PC của mình:
CPU: Intel Core i3 8100
GPU: NVIDIA GTX 750Ti
RAM: 16GB (Dual channel)
SSD: 128 x 3 GB
```

Và mình đã quyết định thử Ubuntu với con máy mới này.

![Ubuntu image](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fitsubuntu.com%2Fwp-content%2Fuploads%2F2022%2F09%2FUbuntu-Unity-Is-Now-Official-Ubuntu-Flavor.jpg&f=1&nofb=1&ipt=21567ca5b4930e879b674a3b248ed815302014378522333382c9b2d4610abef0&ipo=images "Ubuntu") _Ubuntu thì nhìn như thế này._

Dùng Ubuntu mình thấy được cái đẹp hơn Lubuntu (tất nhiên là **bloat** hơn kkk). Mình thấy sử dụng khá ổn, hợp với những người mới tập tành Linux. Thời điểm này mình bắt đầu luyện thêm skill dùng `CLI, git` 🤣.

Một ưu điểm của **Ubuntu** là nó có giao diện **Gnome** rất trực quan. Nếu bạn là người mới, muốn trải nghiệm Linux thì bạn nên bắt đầu với distro này. Bạn sẽ không mất quá nhiều thời gian để làm quen với giao diện đâu. Cá nhân mình thì thấy **Gnome** giống MacOS kiểu gì ấy 😆.

# I use Arch btw 🚀😏

Năm nay mình lên đại học, nên mẹ cho lại con laptop của mẹ. Để mà nói thì nó không phải **siêu mạnh, cấu hình siêu khủng**, nhưng đáp ứng đầy đủ những nhu cầu của mình. Cơ bản thì quan điểm của mình là laptop phải gọn nhẹ, dễ mang vác. Còn muốn cấu hình mạnh thì dùng máy bàn mà quất. Vậy nên mình không thích những con **Laptop Gaming** lắm.

Hè năm nay mình đã chuyển qua dùng Arch linux. Cũng tại mình thấy mọi người nói Arch **cực kì nhẹ**, **cực kì nhanh**. Và sau khi trải nghiệm thì... đúng là thế thật! Không quá khi nói Arch là distro nhẹ nhất của linux (chắc thua mỗi Alpine linux). Và Arch cũng có thể tùy biến sâu nữa, từ chuyên ngành là `ricing` ấy 🤣.

![fastfetch archlinux](/arch.png "fastfetch trên Arch linux của mình") _My Arch Linux_

Mình hiện tại đang dùng Window Manager, cụ thể là i3wm. Ban đầu thì hơi lạ lạ, nhưng khi quen rồi thì thực sự khó bỏ lắm! Nó giúp mình năng suất hơn nhiều luôn ấy. Giờ mình không cần dùng chuột nữa mà tay mình gần như chỉ có gõ phím thôi. Cảm giác nó **_hacker lỏd_** lắm 🤣.

Thời gian này mình học thêm tool như neovim, git, mấy tools trong ngành an toàn thông tin nx,... Tất nhiên mình ở trình độ gà mờ thôi. Nhưng mình vẫn đang cố gắng cải thiện từng ngày. Cá nhân mình thấy Arch thật sự hợp với nhu cầu của mình, nên mình dùng làm hệ điều hành chính luôn.

# Nhược điểm của Linux 😭

Vui vậy thôi nhưng Windows bảo Linux này...

Dù đúng là linux nhẹ hơn, free, tiện cho lập trình, nhưng linux **cực kì tệ** trong khoản **thiết kế, edit, và gaming**

Trước hết thì linux không có các phần mềm của nhà **Adobe**, nên nếu bạn cần Photoshops, Premier Pro, After Effect, thì chỉ có chịu chết 💀. Tất nhiên vẫn có cách để chạy, các bạn có thể dùng máy ảo, hoặc `wine`, nhưng mình thấy cách đó nghèo nghiện quá. Linux có các **alternative** như GIMP, Davinci Resolve, KdenLive, nhưng không hiểu sao mình dùng cứ bị mấy lỗi vớ vẩn. Đơn cử như Davinci Resolve nó cứ không cho dùng GPU để render, rồi nhiều khi còn không hoạt động, crash,... Và mình cũng quen dùng bộ phần mềm của Adobe rồi, vì vậy mình vẫn để Windows dual boot với Arch.😞

![Premiere in arch linux](https://i.redd.it/5yehh3rcxcmc1.png "Minh họa cho việc dùng Premiere trên linux") _Minh họa cho việc dùng Premiere trên linux_

Còn về việc không chơi được nhiều game thì thật ra cũng không ảnh hưởng mình lắm, mình không chơi game quá nhiều 🎮. Nhưng nếu bạn thích chơi game, đặc biệt là mấy game của **Riot** thì hiện tại không chơi được 😥. Dù vậy với vài game chơi được trên linux, mình test thì thấy nó mượt hơn trên windows mọi người ạ, ảo ma vcl. Chắc do nó tận dụng được tài nguyên máy tốt hơn. Và một fun fact: `SteamOS dùng trên Steam Deck là một Linux Distro`.

![Steam OS](https://cdn-media.sforum.vn/storage/app/media/phuoctoan/SteamOS/steam-os-toi-uu-hay-tiec-nuoi-cho-game-thu-9.jpg "SteamOS là Linux Distro") _SteamOS là Linux Distro_

# Bạn có nên dùng Linux 🐧?

Nếu bạn là người dùng bình thường, có máy tính cấu hình ổn, có nhu cầu sử dụng các phần mềm đồ họa, thiết kế và không hứng thú với việc vọc vạch. Thì các bạn không cần thiết sử dụng Linux nhé 😀.

Nếu bạn là sinh viên cntt, người làm trong lĩnh vực công nghệ (các anh các chú các bác trong lĩnh vực này đều biết linux cả rồi nhưng em xin phép cứ liệt kê vào nhé), thì các bạn nên tìm hiểu về Linux. Các bạn có thể sử dụng Window Subsystem for Linux - `WSL`, nếu không muốn phải cài đặt nguyên cả cái hệ điều hành. Như vậy bạn vừa có thể dùng Windows, vừa có thể dùng những tinh túy của Linux 😋.

Hoặc nếu bạn như mình, bạn thích một hệ điều hành **blazingly fast**, thứ mà bạn hoàn toàn có quyền kiểm soát, tùy chỉnh. Bạn đam mê tìm tòi, vọc vạch. Thì Linux chính là hệ điều hành cho bạn 💯.

# Lời kết

Đây là lần đầu mình viết blog, nếu bạn thấy câu từ lủng củng hay thiếu sót gì thì bỏ qua cho mình nha 😆. Hẹn gặp lại các người anh em trong post sau khi nào mình có hứng để viết 🤣.
