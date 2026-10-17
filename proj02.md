**Project thứ 2: Game Oẳn Tù Tì (Rock-Paper-Scissors) Nâng Cao**  
*(Củng cố thêm: hàm, điều kiện, vòng lặp, random, list, tính điểm)*

### Mục tiêu
Bé tự viết một chương trình chơi oẳn tù tì với máy, có điểm số, chơi nhiều ván, và thống kê kết quả. Tập trung thực hành tổ chức code bằng hàm và xử lý logic so sánh.

---

### Yêu cầu bắt buộc (phải có)

1. **Người chơi chọn**  
   - Kéo / Búa / Bao (hoặc 1 = Kéo, 2 = Búa, 3 = Bao).  
   - Kiểm tra nhập sai thì báo lỗi và yêu cầu nhập lại.

2. **Máy chọn ngẫu nhiên**  
   - Dùng `random` để máy chọn Kéo / Búa / Bao.

3. **So sánh kết quả một ván**  
   - Xác định ai thắng, thua hoặc hòa.  
   - In rõ: “Bạn chọn…”, “Máy chọn…”, “Bạn thắng!” / “Bạn thua!” / “Hòa!”.

4. **Tính điểm và chơi nhiều ván**  
   - Thắng +1 điểm, thua 0 điểm (hoặc tự đặt quy tắc).  
   - Hỏi có muốn chơi tiếp không.  
   - Lưu điểm của người chơi và điểm của máy.

5. **Dùng hàm**  
   - Tách ít nhất các phần: chọn của người chơi, chọn của máy, so sánh kết quả, hiển thị bảng điểm.

---

### Yêu cầu nâng cao (làm nếu còn thời gian)
- Lưu lịch sử các ván vào `list` (ví dụ: “Bạn thắng”, “Hòa”, “Máy thắng”).
- Cuối chương trình in thống kê:  
  - Số ván thắng / thua / hòa  
  - Tỷ lệ thắng (%)
- Thêm chế độ “Chơi đến 3 điểm” (ai đạt 3 điểm trước thì thắng).
- Có thông báo vui hoặc emoji đơn giản (nếu muốn).

---

### Gợi ý các bước làm
1. Viết hàm để người chơi nhập lựa chọn (và kiểm tra hợp lệ).
2. Viết hàm để máy chọn ngẫu nhiên.
3. Viết hàm so sánh hai lựa chọn và trả về kết quả.
4. Tạo vòng lặp chính để chơi nhiều ván + cộng điểm.
5. Thêm phần hiển thị điểm hiện tại sau mỗi ván.
6. Cuối cùng in tổng kết.

---

### Ví dụ kết quả khi chạy (để bé hình dung)

```text
=== GAME OẲN TÙ TÌ ===

Ván 1:
Bạn chọn (1=Kéo, 2=Búa, 3=Bao): 2
Bạn chọn: Búa
Máy chọn: Kéo
Bạn thắng!

Điểm hiện tại: Bạn 1 - Máy 0

Bạn có muốn chơi tiếp không? (có/không): có

Ván 2:
Bạn chọn (1=Kéo, 2=Búa, 3=Bao): 3
Bạn chọn: Bao
Máy chọn: Bao
Hòa!

Điểm hiện tại: Bạn 1 - Máy 0

Bạn có muốn chơi tiếp không? (có/không): có

Ván 3:
Bạn chọn (1=Kéo, 2=Búa, 3=Bao): 1
Bạn chọn: Kéo
Máy chọn: Búa
Bạn thua!

Điểm hiện tại: Bạn 1 - Máy 1

Bạn có muốn chơi tiếp không? (có/không): không

=== KẾT QUẢ ===
Tổng số ván: 3
Bạn thắng: 1
Máy thắng: 1
Hòa: 1
Tỷ lệ thắng của bạn: 33.3%
Cảm ơn bạn đã chơi!
```

---

### Tiêu chí hoàn thành
- Chạy được từ đầu đến cuối, không lỗi.
- Có thể chơi nhiều ván và xem điểm.
- Có ít nhất 3 hàm.
- Bé giải thích được logic so sánh thắng/thua.

---
