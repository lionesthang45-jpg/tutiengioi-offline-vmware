# Tu Tiên Giới Offline — VMware Easy2 RC2

**Bộ VMware mới thay thế VMware Lite RC1.** Client + GameServer + website MEL + Liones AI offline, không cần WSL2, Windows OpenSSH hoặc Shared Folders.

## Tải bộ cài mới

**[Tải VMware Easy2 RC2 tại đây](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/tag/v1.6.0-vmware-easy2-rc2-20261018)**

Trong **Assets**, tải đủ **1 EXE + 8 BIN**, khoảng **13,81 GiB (14,83 GB)**. Giữ nguyên tên và để cả 9 file cùng thư mục. Không trộn BIN của VMware Lite hoặc RC1. **Source code (zip/tar.gz) không chứa bộ game để cài.**

| File cần tải | Liên kết |
|---|---|
| Setup | [CaiDat-TuTienGioi-VMware-Easy2-RC2.exe](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.6.0-vmware-easy2-rc2-20261018/CaiDat-TuTienGioi-VMware-Easy2-RC2.exe) |
| Dữ liệu 1 | [RC2-1.bin](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.6.0-vmware-easy2-rc2-20261018/CaiDat-TuTienGioi-VMware-Easy2-RC2-1.bin) |
| Dữ liệu 2 | [RC2-2.bin](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.6.0-vmware-easy2-rc2-20261018/CaiDat-TuTienGioi-VMware-Easy2-RC2-2.bin) |
| Dữ liệu 3 | [RC2-3.bin](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.6.0-vmware-easy2-rc2-20261018/CaiDat-TuTienGioi-VMware-Easy2-RC2-3.bin) |
| Dữ liệu 4 | [RC2-4.bin](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.6.0-vmware-easy2-rc2-20261018/CaiDat-TuTienGioi-VMware-Easy2-RC2-4.bin) |
| Dữ liệu 5 | [RC2-5.bin](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.6.0-vmware-easy2-rc2-20261018/CaiDat-TuTienGioi-VMware-Easy2-RC2-5.bin) |
| Dữ liệu 6 | [RC2-6.bin](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.6.0-vmware-easy2-rc2-20261018/CaiDat-TuTienGioi-VMware-Easy2-RC2-6.bin) |
| Dữ liệu 7 | [RC2-7.bin](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.6.0-vmware-easy2-rc2-20261018/CaiDat-TuTienGioi-VMware-Easy2-RC2-7.bin) |
| Dữ liệu 8 | [RC2-8.bin](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.6.0-vmware-easy2-rc2-20261018/CaiDat-TuTienGioi-VMware-Easy2-RC2-8.bin) |

Đọc `GUI_NGUOI_CHOI.txt`, `CHUAN_BI_VMWARE.txt` và `QA-KET_QUA.txt`. `DOWNLOAD_SHA256SUMS.txt` có SHA của tất cả file phát hành (trừ chính file checksum); `SHA256SUMS.txt` đối chiếu 9 file cài đặt. Bộ cài chưa có chữ ký số; checksum không thay thế xác thực nhà phát hành.

## Cài một lần, sau đó Chơi ngay

1. Windows 10/11 **x64**, bật ảo hóa CPU trong BIOS. Khuyến nghị RAM **12–16 GiB trở lên**. Máy ảo dùng **4 GiB RAM / 2 vCPU**. Máy 8 GiB có cảnh báo và chưa bảo đảm chạy đủ game + AI trên mọi cấu hình.
2. Chạy EXE. Nếu chưa có VMware, bấm **TẢI VMWARE CHÍNH THỨC**, tự tải/cài Workstation Pro từ [Broadcom](https://knowledge.broadcom.com/external/article/368734/download-desktop-hypervisor-workstation.html), rồi quay lại **ĐÃ CÀI VMWARE — KIỂM TRA**. Không kèm bộ cài VMware trong bộ game.
3. Máy đã có VMware/Jx khác: bấm **ĐÃ CÀI VMWARE — KIỂM TRA**. Setup kiểm tra thực tế, không chỉ ghi nhận nút bấm. Có thể tự khởi động dịch vụ VMware/bật đúng adapter cần thiết sau UAC, giữ nguyên các mạng/port forwarding của Jx khác.
4. Chọn **thư mục trống**; không cài đè bản có nhân vật. Nội dung mới khoảng **20,03 GiB**, chưa tính bộ EXE/BIN và file RAM/dữ liệu tăng khi chơi. Nên chừa khoảng **40 GB trống** trên ổ cài game; có thể chọn ổ D/E/F.
5. Giữ tùy chọn mở Launcher sau cài đặt: chương trình kiểm tra khởi động Linux, Tools, SSH, Server và AI thật. Chờ **HOÀN TẤT**, rồi **CHƠI NGAY**. Lần đầu có thể lâu; không bấm lặp.
6. Tài khoản mẫu kiểm thử **gm / 1**. Website dùng quản lý nhân vật; thêm tên trên website **không** tạo tài khoản đăng nhập game.
7. Khi nghỉ: thoát Client → **DỪNG AN TOÀN** → đợi hoàn tất → tắt Windows. Đóng Launcher không tự tắt Server.

BIOS, xác nhận UAC, khởi động lại Windows hoặc wizard sửa driver VMware cần chủ máy thực hiện. Nếu driver/cả hai mạng dùng chung bị hỏng cấu hình, không tự reset tất cả để làm hỏng các Jx khác; xem hướng dẫn chuẩn bị. Nếu phải chuẩn bị lại VMware, dùng `ChuanBi-VMware.cmd` hoặc nút trong Launcher, **không xóa/cài lại game**.

## Cổng, AI và WinSCP

- Cổng mặc định bị chiếm: chọn cổng trống, đồng bộ Client/guest/website/AI. Bấm **MỞ WEBSITE** để vào đúng cổng; không ép `127.0.0.1:80`. Không kill ứng dụng khác hoặc xóa NAT để giành cổng.
- Ưu tiên NAT/VMnet8 đang tốt, có thể tự chọn Host-only/VMnet1 phù hợp cho riêng VM của bản này. Không ép mọi máy về cùng IP và không tự Restore Defaults VMware.
- AI mặc định **Tự động + qwen3:1.7b nhẹ**; có CPU/GPU và chuyển về CPU nếu GPU không dùng được. Model 8b tùy chọn cần nhiều RAM hơn, chưa chạy lại end-to-end cho RC2. Tốc độ tùy máy.
- **WINSCP / SỬA FILE** mở thông tin kết nối riêng: IP hiện tại, root, cổng, khóa và thư mục server. Chỉ cần Linux chạy, không cần GameServer/AI chạy. WinSCP cài riêng từ [trang chính thức](https://winscp.net/eng/download.php).
- Người chơi có quyền root chỉnh server; không thêm DRM/kích hoạt online. Dừng server và sao lưu trước khi sửa. Không dùng IP/mật khẩu trên ảnh của người khác, không chia sẻ private key/profile/database lên nhóm hoặc GitHub.

## Người đã có bản cũ

RC2 là **bộ cài mới riêng**, chưa tự chuyển nhân vật từ VMware Lite/WSL2. **Giữ nguyên bản cũ nếu cần nhân vật**, không cài đè, không xóa VMDK/JSON để thử lại. VMware Lite RC1 đã được thay thế cho lượt tải/cài mới; bản cũ trong lịch sử chỉ để đối chiếu/dự phòng, không trộn file với RC2.

## Phạm vi nghiệm thu

**RC2, chưa phải Final cho mọi máy.** Đã kiểm trên máy dựng bằng đúng EXE/BIN cuối: 8.471 SHA payload, cấm cài đè, đường dẫn có dấu/khoảng trắng/ngoặc, cổng bị chiếm, CPU fallback thật, native heartbeat/probe/map, WinSCP.com thật, di chuyển giữ identity/key, dừng qua Tools khi thiếu khóa SSH, và mạng VMware dùng chung không đổi. Nút xác nhận VMware đã bấm thử trên Setup thật. 26 tình huống chuẩn bị là **mô phỏng**, không phải 26 máy vật lý; bộ thực thi tự sửa được thử với các thao tác OS mô phỏng, không cố tình phá mạng máy dựng.

Còn cần nhóm test xác nhận đăng nhập/tạo nhân vật/relogin, chat/F3/Tống Kim/map/thú cưỡi và thao tác Launcher/WinSCP trên desktop. Nếu lỗi, dùng **GÓI HỖ TRỢ** và gửi ZIP mới cho người hỗ trợ tin cậy. Không Power Off/Reset hoặc xóa database để thử.

Kho này chỉ chứa tài liệu và các gói đã niêm phong; không đăng dữ liệu QA đang chơi, private key hoặc profile của máy dựng. Thông báo/giấy phép thành phần nằm trong bộ cài và `ThirdPartyLicenses.zip`.
