# Sổ Giờ Học

Ứng dụng bấm giờ học theo từng môn, kèm chỉ tiêu (KPI) ngày/tuần. Toàn bộ app nằm trong một file `index.html` duy nhất — không cần cài đặt, không cần máy chủ.

## Chức năng

- **Bộ đếm riêng cho từng môn học.** Bấm ▶ để bắt đầu học, bấm ⏸ để dừng. Bắt đầu một môn sẽ tự dừng môn đang chạy, vì mỗi lúc chỉ học một môn.
- **Thống kê hôm nay và tổng cộng** cho từng môn cùng tổng chung của cả sổ.
- **KPI theo ngày hoặc theo tuần.** Đặt chỉ tiêu số giờ cho từng môn; thanh tiến độ hiện ngay dưới tên môn và đóng dấu *ĐẠT* khi đủ giờ.
- **Chấm chỉ tiêu khi kỳ khép lại.** Mở app lên, nếu có ngày/tuần vừa kết thúc thì hiện bảng tổng kết đạt hay không đạt.
- **Nhận xét sau mỗi 3 kỳ liên tiếp.** Ba kỳ trượt liên tiếp sẽ nhận lời cảnh báo nghiêm khắc; ba kỳ đạt liên tiếp sẽ nhận lời ghi nhận.
- **Chế độ Sáng / Tối / Tự động** — chế độ tự động dùng nền sáng từ 6:00 đến 18:00 và nền tối từ 18:00 đến 6:00.
- **Sao lưu và khôi phục** dữ liệu bằng file `.json`.

## Cách dùng

Mở `index.html` bằng trình duyệt là chạy được ngay. Trên Windows có thể tạo shortcut mở ở chế độ cửa sổ riêng:

```
msedge.exe --app="file:///<đường-dẫn>/index.html"
```

## Dữ liệu

Dữ liệu giờ học được lưu bằng `localStorage` của trình duyệt, nằm trên chính máy người dùng và không gửi đi đâu cả. Mỗi máy, mỗi trình duyệt là một bộ dữ liệu riêng. Xoá dữ liệu duyệt web sẽ xoá luôn lịch sử giờ học, nên hãy dùng nút **Lưu bản sao dữ liệu** định kỳ.
