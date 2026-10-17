**Đề bài: Game Đoán Số Nâng Cao**  
*(Dành cho tối nay – khoảng 60–90 phút thực hành)*

### Mục tiêu
Bé tự viết một chương trình game đoán số hoàn chỉnh, dùng nhiều kiến thức đã học (biến, điều kiện, vòng lặp, hàm, `random`, có thể dùng list). Không copy code nguyên xi từ nguồn khác.

---

### Yêu cầu bắt buộc (phải có)

1. **Chọn mức độ khó**
   - Dễ: số từ 1–50
   - Trung bình: số từ 1–100
   - Khó: số từ 1–200  
   Người chơi chọn mức trước khi bắt đầu ván.

2. **Cách chơi một ván**
   - Máy chọn ngẫu nhiên một số trong khoảng đã chọn.
   - Người chơi đoán số.
   - Mỗi lần đoán sai, chương trình báo: **“Cao hơn”** hoặc **“Thấp hơn”**.
   - Đếm số lần đoán.
   - Khi đoán đúng → in ra “Đúng rồi! Bạn đoán trong X lần”.

3. **Tính điểm**
   - Đoán càng ít lần thì điểm càng cao.  
     Ví dụ gợi ý: điểm = (số lớn nhất của mức) − (số lần đoán × 5)  
     (Bé có thể tự nghĩ công thức khác, miễn hợp lý).

4. **Chơi nhiều ván**
   - Sau mỗi ván, hỏi “Bạn có muốn chơi tiếp không? (có/không)”.
   - Lưu **điểm cao nhất** trong phiên chơi (chỉ cần biến, chưa cần lưu file).

5. **Dùng hàm**
   - Ít nhất phải tách thành 2–3 hàm riêng (ví dụ: hàm chọn mức độ, hàm chơi một ván, hàm tính điểm…).

---

### Yêu cầu nâng cao (làm nếu còn thời gian)
- Lưu lịch sử điểm của các ván vào một `list`.
- Cuối chương trình in ra:
  - Điểm cao nhất
  - Trung bình điểm các ván đã chơi
- Giới hạn số lần đoán tối đa (ví dụ tối đa 10 lần, quá thì thua).
- Thêm thông báo vui khi đoán đúng (ví dụ “Giỏi quá!”, “Bạn là cao thủ!” tùy số lần đoán).

---

### Gợi ý các bước làm (không bắt buộc theo đúng thứ tự)
1. Viết phần chọn mức độ khó và in ra khoảng số.
2. Viết hàm chơi một ván (dùng `while` để đoán đến khi đúng).
3. Thêm tính điểm.
4. Bọc vào vòng lặp chính để chơi nhiều ván.
5. Thêm lưu điểm cao nhất.
6. Tách code thành các hàm cho gọn.
7. Test thử nhiều lần, sửa lỗi.

---

### Tiêu chí hoàn thành tối nay
- Chương trình chạy được từ đầu đến cuối không bị lỗi.
- Người chơi có thể chọn mức độ, đoán số, xem điểm, chơi nhiều ván.
- Có ít nhất 2 hàm.
- Bé có thể giải thích được từng phần code làm gì.

---

### Công cụ
Dùng **Thonny** hoặc **Replit**. Nhớ `import random` ở đầu file.

---

=== GAME ĐOÁN SỐ ===

Chọn mức độ khó:
1. Dễ (1 - 50)
2. Trung bình (1 - 100)
3. Khó (1 - 200)
Nhập lựa chọn (1/2/3): 2

Bạn đã chọn mức Trung bình. Hãy đoán số từ 1 đến 100!

Lần đoán thứ 1: 50
Thấp hơn!

Lần đoán thứ 2: 75
Cao hơn!

Lần đoán thứ 3: 62
Thấp hơn!

Lần đoán thứ 4: 68
Đúng rồi! Bạn đoán trong 4 lần.
Bạn được 80 điểm.

Bạn có muốn chơi tiếp không? (có/không): có

Chọn mức độ khó:
1. Dễ (1 - 50)
2. Trung bình (1 - 100)
3. Khó (1 - 200)
Nhập lựa chọn (1/2/3): 1

Bạn đã chọn mức Dễ. Hãy đoán số từ 1 đến 50!

Lần đoán thứ 1: 25
Cao hơn!

Lần đoán thứ 2: 10
Đúng rồi! Bạn đoán trong 2 lần.
Bạn được 40 điểm.
Giỏi quá!

Bạn có muốn chơi tiếp không? (có/không): không

=== KẾT QUẢ PHIÊN CHƠI ===
Điểm cao nhất: 80 điểm
Các ván đã chơi: 80, 40
Trung bình điểm: 60.0
Cảm ơn bạn đã chơi!
