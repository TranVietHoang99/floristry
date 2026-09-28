# 💐 Floristry

Game **Floristry** (David Gordon & TAM, Uncommons Publishing) cho 2 người, chơi ngay trên trình duyệt: đấu giá hoa kiểu Hà Lan rồi xếp domino hoa vào tủ kính.

## Chế độ chơi
- **Chơi với máy**: nhập tên, bấm *Chơi với máy*.
- **Online 1 đấu 1**: bấm *Tạo phòng*, gửi mã hoặc link cho bạn bè; bạn bè nhập mã và bấm *Vào phòng*.
  Người tạo phòng phải **giữ tab mở**, vì máy chủ phòng giữ trạng thái và chạy đồng hồ đấu giá.

## Luật tóm tắt (theo rulebook v1.6)
10 vòng, mỗi vòng:
1. **Chợ**: rút 4 ô domino hoa (2 bông mỗi ô, có thể khác loại).
2. **Đấu giá**: cả hai bấm *Sẵn sàng*. Trong 15 giây, giá bắt đầu $5 và giảm $1 mỗi 3 giây.
   Ai bấm **MUA** trước trả giá hiện tại và chọn 3 ô; người kia nhận ô còn lại miễn phí. Không ai mua thì bỏ cả 4 ô.
3. **Trang trí**: cả hai cùng lúc đặt ô mới vào tủ kính. Được xoay, phải chạm cạnh ô cũ, không được dời ô cũ.

Điểm: mỗi loại hoa chỉ tính mảng lớn nhất: 3–5 = 1, 6–8 = 3, 9–11 = 6, 12+ = 10.
Mỗi người bắt đầu với $30; ai nhiều tiền hơn cuối trận được điểm theo mức chênh lệch, tính theo cùng bảng trên.

## Phần tự quyết (rulebook không ghi rõ)
- Khung tủ kính là lưới **8×6** ô. Được "trượt khung": đặt ô ra hàng/cột mép ngoài thì cả tủ tự dịch vào nếu còn chỗ.
- Bộ 42 ô: 6 ô đôi cùng loại + 36 ô hai loại khác nhau, mỗi loại hoa đúng 14 bông.
- Ô không còn chỗ đặt thì phải bỏ.

## Cách bấm
- Đấu giá: nút **MUA** (hoặc phím Space).
- Trang trí: chọn ô trong giỏ, rê chuột lên tủ kính để xem trước (xanh = hợp lệ), bấm để đặt.
  Xoay bằng nút ⟳, chuột phải, phím R, hoặc bấm lại vào ô đang chọn. Có *Hoàn tác* trước khi *Xác nhận*.
- Rê chuột lên một loại hoa ở bảng điểm để tô sáng mảng lớn nhất.

## Kỹ thuật
Một file `index.html` duy nhất. Kết nối P2P bằng [PeerJS](https://peerjs.com/), cùng khung với Jaipur và 7 Wonders Duel.
Chạy thử: `npx http-server floristry -p 5181`.
