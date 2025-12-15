# TTNT
> Kho mã này tổng hợp 03 bài thực hành, được xây dựng tập trung vào tối ưu hóa thuật toán, cấu trúc mã rõ ràng (function, class), và hỗ trợ giao diện tương tác.

## MỤC LỤC

1.  [Bài 1: Giải Sudoku bằng thuật toán quay lui (Tuan3)](#1-bài-1-giải-sudoku-bằng-thuật-toán-quay-lui-tuan3)
2.  [Bài 2: Bài toán tô màu đồ thị (Tuan4)](#2-bài-2-bài-toán-tô-màu-đồ-thị-tuan4)
3.  [Bài 3: Bài toán người du lịch (TSP - Tuan5)](#3-bài-3-bài-toán-người-du-lịch-tsp---tuan5)
4.  [Hướng dẫn chạy & yêu cầu demo](#4-hướng-dẫn-chạy--yêu-cầu-demo)

---

## 1. Bài 1: Giải Sudoku bằng thuật toán quay lui (Tuan3)

**Tệp mã nguồn:** `Tuan3.ipynb`

### Mục tiêu & Phương pháp
* **Mục tiêu:** Tìm kiếm lời giải cho bảng Sudoku.
* **Phương pháp:** Sử dụng **Thuật toán Quay lui (Backtracking)**. Đây là một phương pháp tìm kiếm vét cạn có tổ chức, thuật toán thử đặt một số hợp lệ vào ô trống và quay lui khi không tìm thấy lời giải tiếp theo. 
* **Cấu trúc Code:** Mã nguồn được định nghĩa rõ ràng bằng các **hàm (function)** như `is_safe` (kiểm tra tính hợp lệ của số được đặt), `find_empty_location` (tìm ô trống tiếp theo), và `solve_sudoku` (hàm chính thực hiện quay lui), đảm bảo tính tối ưu và dễ đọc.

### Tính năng Demo (Input Động)
Để đáp ứng yêu cầu demo tương tác, chương trình cho phép người dùng **nhập vào ma trận Sudoku ban đầu** dưới dạng List of Lists trong một cell input. Điều này chứng minh khả năng xử lý **thông số động**.

**Ví dụ Input (Người dùng có thể thay đổi ma trận này):**
```python
# Mở cell code và thay đổi input:
board = [
    [5, 3, 0, 0, 7, 0, 0, 0, 0],
    [6, 0, 0, 1, 9, 5, 0, 0, 0],
    # ... (Các hàng khác)
    [0, 0, 0, 0, 8, 0, 0, 7, 9]
]
