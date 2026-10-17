**Project thứ 3: Game Hangman (Đoán từ)**  
*(Củng cố mạnh: chuỗi, list, vòng lặp, điều kiện, hàm, xử lý ký tự)*

### Mục tiêu
Bé tự viết game đoán từ (treo cổ). Người chơi đoán từng chữ cái của một từ bí mật. Tập trung thực hành xử lý chuỗi và list.

---

### Yêu cầu bắt buộc (phải có)

1. **Từ bí mật**
   - Có sẵn một danh sách từ (ít nhất 5–10 từ) trong chương trình.
   - Máy chọn ngẫu nhiên một từ để chơi.

2. **Hiển thị từ đang đoán**
   - Ban đầu hiện dạng ` _ _ _ _ ` (mỗi dấu `_` là một chữ cái).
   - Mỗi lần đoán đúng thì hiện chữ cái đó ra đúng vị trí.

3. **Cách chơi**
   - Người chơi nhập từng chữ cái.
   - Kiểm tra chữ cái đã đoán chưa (không cho đoán trùng).
   - Nếu đúng → cập nhật từ hiển thị.
   - Nếu sai → trừ số lần còn lại (ví dụ bắt đầu với 6–7 lần sai).

4. **Kết thúc ván**
   - Đoán đúng hết từ → thắng.
   - Hết lượt sai → thua, hiện ra từ đúng.
   - In thông báo rõ ràng.

5. **Dùng hàm**
   - Tách các phần: chọn từ, hiển thị từ, kiểm tra đoán, cập nhật trạng thái…

---

### Yêu cầu nâng cao (làm nếu còn thời gian)
- Có hình “treo cổ” đơn giản bằng text (mỗi lần sai thêm một phần thân).
- Lưu các chữ cái đã đoán (đúng và sai) để hiển thị.
- Cho phép chơi nhiều từ liên tiếp.
- Thêm mức độ khó (từ ngắn / từ dài).
- Cuối cùng thống kê số từ đoán đúng.

---

### Gợi ý các bước làm
1. Tạo danh sách từ và hàm chọn từ ngẫu nhiên.
2. Tạo list hoặc chuỗi để theo dõi các chữ cái đã hiện.
3. Viết hàm hiển thị từ hiện tại (dạng `_ a _ _`).
4. Viết vòng lặp chính: nhập chữ cái → kiểm tra → cập nhật.
5. Kiểm tra điều kiện thắng/thua.
6. Tách thành các hàm cho code sạch.

---

### Ví dụ kết quả khi chạy (để bé hình dung)

```text
=== GAME HANGMAN ===

Từ có 5 chữ cái. Bạn có 6 lần đoán sai.

Từ: _ _ _ _ _
Chữ cái đã đoán: 
Lần còn lại: 6

Nhập chữ cái: a
Đúng!

Từ: _ a _ _ _
Chữ cái đã đoán: a
Lần còn lại: 6

Nhập chữ cái: e
Sai!

Từ: _ a _ _ _
Chữ cái đã đoán: a e
Lần còn lại: 5

Nhập chữ cái: p
Đúng!

Từ: _ a p _ _
Chữ cái đã đoán: a e p
Lần còn lại: 5

Nhập chữ cái: l
Đúng!

Từ: _ a p l _
Chữ cái đã đoán: a e p l
Lần còn lại: 5

Nhập chữ cái: e
Bạn đã đoán chữ này rồi!

Nhập chữ cái: p
Bạn đã đoán chữ này rồi!

Nhập chữ cái: p
Bạn đã đoán chữ này rồi!

Nhập chữ cái: y
Đúng!

Từ: _ a p p y
Chúc mừng! Bạn đã đoán đúng từ: happy
```

*(Hoặc nếu thua sẽ hiện: “Bạn đã thua! Từ đúng là: python”)*

---

### Tiêu chí hoàn thành
- Chạy được hoàn chỉnh một ván.
- Hiện đúng các chữ cái đã đoán và số lần còn lại.
- Có ít nhất 3 hàm.
- Bé giải thích được cách cập nhật từ hiển thị.

---
