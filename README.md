# SO SÁNH TRADE-OFF CÁC GIẢI PHÁP PROMPTING
## Chủ đề: Ứng dụng AI trong Học tập & Nghiên cứu

## Bước 1: Đề xuất 2 prompt mẫu

### Giải pháp 1: Prompt đơn giản

Bạn là AI gia sư. Hãy giải thích [CHỦ_ĐỀ] theo phương pháp Feynman bằng ngôn ngữ dễ hiểu. Sau đó chấm [BÀI_LÀM] theo [RUBRIC], đưa ra điểm số và nhận xét ngắn gọn.

### Giải pháp 2: Prompt chi tiết

Bạn là AI gia sư và trợ lý chấm bài.

**Yêu cầu:**
1. Giải thích [CHỦ_ĐỀ] theo phương pháp Feynman, phù hợp với [TRÌNH_ĐỘ].
2. Chấm [BÀI_LÀM] theo từng tiêu chí trong [RUBRIC].
3. Tính tổng điểm và nhận xét ưu, nhược điểm.
4. Đề xuất cách cải thiện bài làm.

**Điều kiện:**
- Nếu thiếu dữ liệu, yêu cầu người dùng bổ sung.
- Nếu bài làm trống, không chấm điểm.
- Nếu Rubric không rõ ràng, thông báo lỗi.
- Không tự ý thêm tiêu chí hoặc bịa điểm.
- Trình bày kết quả bằng Markdown.

## Bước 2: Bảng so sánh Trade-off

| Tiêu chí | Giải pháp 1 (Đơn giản) | Giải pháp 2 (Chi tiết) |
|---|---|---|
| Độ dễ hiểu | Cao | Trung bình |
| Tốn token | Ít | Nhiều hơn |
| Tốc độ xử lý | Nhanh | Chậm hơn |
| Độ chính xác | Khá | Cao |
| Chặn lỗi biên | Trung bình | Rất tốt |
| Khả năng tái sử dụng | Trung bình | Cao |

## Bước 3: Lựa chọn và chạy thử

**Lựa chọn:** Giải pháp 2.

**Lý do:** Có hướng dẫn rõ ràng, xử lý được dữ liệu thiếu hoặc sai lệch, giúp kết quả giải thích và chấm điểm nhất quán hơn.

### Chạy thử

**Input:**
- [CHỦ_ĐỀ]: Biến trong lập trình C.
- [TRÌNH_ĐỘ]: Sinh viên năm nhất.
- [BÀI_LÀM]: Biến dùng để lưu trữ dữ liệu.
- [RUBRIC]: Kiến thức đúng (5 điểm), giải thích dễ hiểu (3 điểm), ví dụ (2 điểm).

**Kết quả AI:**

**1. Giải thích Feynman:**

Biến giống như một chiếc hộp dùng để lưu trữ dữ liệu. Ví dụ: `int tuoi = 18;` nghĩa là tạo biến `tuoi` để lưu số nguyên 18.

**2. Chấm điểm:**

| Tiêu chí | Điểm |
|---|---:|
| Kiến thức đúng | 5/5 |
| Giải thích dễ hiểu | 3/3 |
| Ví dụ | 0/2 |
| **Tổng điểm** | **8/10** |

**3. Nhận xét:**

Ưu điểm: Nêu đúng chức năng của biến.

Hạn chế: Chưa có ví dụ minh họa.

Cải thiện: Bổ sung ví dụ khai báo biến trong C.

## Kết luận

Giải pháp 2 tối ưu hơn vì kiểm soát đầu vào, hạn chế lỗi và tạo kết quả đầy đủ, nhất quán. Dù tốn nhiều token hơn, phương án này phù hợp với quy trình gia sư và chấm bài tự động.
