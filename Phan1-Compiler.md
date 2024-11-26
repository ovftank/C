# Mở đầu

## Giới thiệu về Trình Biên Dịch

### 1. Trình biên dịch là gì?

Để thực thi một chương trình viết bằng `ngôn ngữ C`, chúng ta cần sử dụng `trình biên dịch`. `Trình biên dịch` là một phần mềm được sử dụng để chuyển đổi mã nguồn của chương trình từ ngôn ngữ lập trình sang mã máy có thể thực thi được trên máy tính, điện thoại hoặc các thiết bị khác.

Các ngôn ngữ lập trình khác như `Python` và `Java` sử dụng `trình thông dịch` và `máy ảo` để thực thi chương trình. Chúng ta sẽ tìm hiểu về cái này sau.

### 2. Cách cài đặt trình biên dịch

Có nhiều cách để cài đặt trình biên dịch cho `ngôn ngữ C` trên hệ điều hành Windows. Tuy nhiên, một cách đơn giản là sử dụng trình quản lý gói `Chocolatey`.

Để cài đặt `Chocolatey` (nếu chưa có), làm theo các bước sau trong `Powershell` với quyền quản trị:

```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```

1. Mở `Command Prompt` với quyền quản trị (Run as Administrator).

2. Cài đặt `MinGW` (Minimalist GNU for Windows), bằng cách chạy lệnh sau:

    ```powershell
    choco install mingw
    ```

    ***Trên hệ điều hành Arch Linux, chúng ta không cần cài đặt MinGW như trên Windows, mà thay vào đó, chúng ta cài đặt gói `base-devel` bao gồm trình biên dịch `gcc` trên hệ điều hành Arch Linux:***

    ```bash
    sudo pacman -Syyu base-devel
    ```

3. Sau khi cài đặt xong, đóng `Command Prompt` và mở lại để cập nhật các biến môi trường.

4. Kiểm tra xem `MinGW` đã được cài đặt thành công bằng cách chạy lệnh sau:

    ```powershell
    gcc --version
    ```

    Nếu lệnh trên hiển thị phiên bản của trình biên dịch `GCC` (GNU Compiler Collection), tức là MinGW đã được cài đặt thành công.

### Sử dụng

- Biên dịch mã nguồn C:

    ``` bash
    gcc source.c -o output
    ```

    Trong đó:

    `source.c`: Tên của tệp mã nguồn C bạn muốn biên dịch.

    `-o output`: Đặt tên cho tệp thực thi sau khi biên dịch ***(nếu là windows thì thêm đuôi.exe vào cuối)***
- ***Trong thực tế, để biên dịch một chương trình viết bằng ngôn ngữ C ta cần biên dịch từng tệp thành các đối tượng, sau đó liên kết chúng lại, để tự động hoá thì chúng ta sẽ sử dụng Makefile, mình sẽ hướng dẫn phần này sau***

[Phần 2 - Chương trình đầu tiên](/C/Phan2-HelloWorld)
