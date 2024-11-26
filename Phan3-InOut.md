# Nhập xuất trong C

## Printf

### 2.1. Cú pháp `printf`

- `printf` được sử dụng để hiển thị thông tin ra màn hình.
- Cú pháp:

```c
printf("format_string", arguments);
```

- Trong đó, `"format_string"` là chuỗi định dạng để xác định cách in các giá trị.
- `arguments` là các giá trị hoặc biểu thức muốn in ra màn hình.

### 2.2. Ví dụ sử dụng `printf`

- Ví dụ: In ra một số nguyên và một chuỗi.
- Mã nguồn:

```c
int num = 10;
char str[] = "Hello, world!";
printf("Số nguyên: %d\nChuỗi: %s\n", num, str);
```

- Kết quả:

```bash
Số nguyên: 10
Chuỗi: Hello, world!
```

## Scanf

### 3.1. Cú pháp `scanf`

- `scanf` được sử dụng để đọc dữ liệu từ người dùng qua bàn phím.
- Cú pháp:

```c
scanf("format_string", arguments);
```

- Trong đó, `"format_string"` là chuỗi định dạng mô tả kiểu dữ liệu của các biến muốn đọc.
- `arguments` là các biến muốn lưu trữ giá trị nhập từ người dùng.

### 3.2. Ví dụ sử dụng `scanf`

- Ví dụ: Đọc một số nguyên từ người dùng.
- Mã nguồn:

```c
int num;
printf("Nhập một số nguyên: ");
scanf("%d", &num);
printf("Số nguyên đã nhập: %d\n", num);
```

- Trong ví dụ trên, `%d` trong chuỗi định dạng của `scanf` cho biết muốn đọc một số nguyên.
- Biến `num` được truyền vào `scanf` bằng cách sử dụng toán tử `&` để truyền địa chỉ của biến.

[<- Phần 2 - Mở đầu](/Phan2-HelloWorld)
