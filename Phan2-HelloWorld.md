# Chương trình đầu tiên

## 1.1. Mở trình soạn thảo văn bản và tạo tệp mới

- Mở trình soạn thảo văn bản như Vim, Visual Studio Code, Sublime Text, vv.
- Tạo một tệp mới.

## 1.2. Nhập mã nguồn vào tệp

- Sao chép đoạn mã nguồn C sau và dán vào tệp:

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

## 1.3. Giải thích mã nguồn

- `#include <stdio.h>`: Lệnh tiền xử lý để đưa thư viện chuẩn vào chương trình. Thư viện này chứa hàm `printf` được sử dụng để in chuỗi ra màn hình.
- `main()`: Hàm chính của chương trình, nơi bắt đầu thực thi mã C.
- `printf("Hello, World!\n");`: In chuỗi "Hello, World!" ra màn hình. `"\n"` là ký tự xuống dòng.
- `return 0;`: Kết thúc hàm `main` và trả về giá trị 0 để biểu thị chương trình đã kết thúc thành công.

## 1.4. Lưu tệp với phần mở rộng `.c`

- Lưu tệp với phần mở rộng `.c`, ví dụ: `main.c`.

## 1.5. Biên dịch và chạy chương trình

- Mở một trình biên dịch C như GCC, Clang.
- Biên dịch tệp `.c` thành một tệp thực thi, ví dụ `.exe` trên Windows, bằng cách chạy lệnh sau trong dòng lệnh:

```bash
gcc main.c -o main.exe
```

- Chạy tệp thực thi bằng cách gõ tên tệp thực thi vào dòng lệnh:

```bash
main.exe
```

- Sau khi chạy, chuỗi "Hello, World!" sẽ được in ra màn hình.

Đó là cách viết và biên dịch chương trình "Hello, World!" trong ngôn ngữ C.

[Phần 3 - Nhập xuất trong C](https://github.com/tripleseven190504/c/blob/main/Phan3-InOut.md)
