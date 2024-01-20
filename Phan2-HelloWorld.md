# Chương trình đầu tiên

Bước 1: Mở trình soạn thảo văn bản (ví dụ: Vim, Visual Studio Code, Sublime Text,...) và tạo một tệp mới.

Bước 2: Nhập mã nguồn sau vào tệp:

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

Trong đoạn mã này, `#include <stdio.h>` là một lệnh tiền xử lý (preprocessor directive) dùng để đưa vào thư viện chuẩn của ngôn ngữ C, trong đó có hàm `printf` được sử dụng để in chuỗi ký tự ra màn hình.

Hàm `main` là hàm chính của chương trình. Mọi mã chương trình C bắt đầu thực thi từ hàm `main`.

Dòng `printf("Hello, World!\n");` in ra chuỗi "Hello, World!" trên màn hình. `"\n"` là ký tự xuống dòng để xuống dòng mới sau khi in chuỗi.

Dòng `return 0;` dùng để kết thúc hàm `main` và trả về giá trị 0 để cho biết chương trình đã kết thúc thành công.

Bước 3: Lưu tệp với phần mở rộng `.c` (ví dụ: `main.c`).

Bước 4: Mở một trình biên dịch C (ví dụ: GCC, Clang) và biên dịch tệp `.c` thành một tệp thực thi (ví dụ: `.exe` trên Windows) bằng cách chạy lệnh sau trong dòng lệnh:

``` bash
gcc main.c -o main.exe
```

Lệnh trên sẽ biên dịch tệp `main.c` và tạo ra tệp thực thi `main.exe`.

Bước 5: Chạy tệp thực thi bằng cách gõ tên tệp thực thi vào dòng lệnh:

```bash
main.exe
```

Sau khi chạy, bạn sẽ nhìn thấy chuỗi "Hello, World!" được in ra màn hình.

Đó là cách bạn có thể viết và biên dịch chương trình "Hello, World!" trong ngôn ngữ C.
