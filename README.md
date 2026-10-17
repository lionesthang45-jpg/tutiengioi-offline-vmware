# Tu Tiên Giới Offline — VMware Lite

Bộ cài đầy đủ **Client + GameServer VMware + website MEL + Liones AI**, không dùng WSL2. Đây là **Lite RC1 gửi kiểm thử**, chưa gọi Final trên mọi cấu hình.

## Tải bộ cài

**[Mở trang tải VMware Lite RC1](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/tag/v1.5.0-vmware-lite-rc1-20261017)**

Trong mục **Assets**, tải đủ **1 EXE và 7 BIN** dưới đây, để tất cả trong cùng một thư mục. Tổng bộ cài khoảng12 GiB. Không đổi tên file, không trộn BIN của bản cũ.

| File | Tải trực tiếp |
|---|---|
| Bộ cài EXE | [CaiDat-TuTienGioi-VMware-Lite-RC1.exe](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.5.0-vmware-lite-rc1-20261017/CaiDat-TuTienGioi-VMware-Lite-RC1.exe) |
| Dữ liệu1 | [RC1-1.bin](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.5.0-vmware-lite-rc1-20261017/CaiDat-TuTienGioi-VMware-Lite-RC1-1.bin) |
| Dữ liệu2 | [RC1-2.bin](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.5.0-vmware-lite-rc1-20261017/CaiDat-TuTienGioi-VMware-Lite-RC1-2.bin) |
| Dữ liệu3 | [RC1-3.bin](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.5.0-vmware-lite-rc1-20261017/CaiDat-TuTienGioi-VMware-Lite-RC1-3.bin) |
| Dữ liệu4 | [RC1-4.bin](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.5.0-vmware-lite-rc1-20261017/CaiDat-TuTienGioi-VMware-Lite-RC1-4.bin) |
| Dữ liệu5 | [RC1-5.bin](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.5.0-vmware-lite-rc1-20261017/CaiDat-TuTienGioi-VMware-Lite-RC1-5.bin) |
| Dữ liệu6 | [RC1-6.bin](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.5.0-vmware-lite-rc1-20261017/CaiDat-TuTienGioi-VMware-Lite-RC1-6.bin) |
| Dữ liệu7 | [RC1-7.bin](https://github.com/lionesthang45-jpg/tutiengioi-offline-vmware/releases/download/v1.5.0-vmware-lite-rc1-20261017/CaiDat-TuTienGioi-VMware-Lite-RC1-7.bin) |

Tải thêm `BAT_DAU_O_DAY.txt`, `KIEM_THU.txt` và `ThirdPartyLicenses.zip`. Có checksum để kiểm file tải lỗi. **Không tải “Source code (zip)” để cài game**: đó chỉ là tài liệu kho GitHub, không chứa bộ game.

## Cài và chơi

1. Máy cần Windows x64, VMware Workstation và ảo hóa BIOS. Windows cần **OpenSSH Client**: mở Settings, tìm Optional features, thêm OpenSSH Client nếu chưa có. Đây là công cụ để Launcher nối vào máy ảo, không phải tài khoản game.
2. Tải đủ EXE+7BIN, chạy EXE, chọn **thư mục trống**. Payload mới cài khoảng18,64 GiB, còn tăng khi chơi; cần chừa thêm dung lượng cho bộ tải12 GiB và dữ liệu phát sinh.
3. Mở **JxLTLauncher - VMware Lite** trên Desktop → **CHƠI NGAY**, chờ Server+AI sẵn sàng.
4. Tài khoản mẫu **gm / 1**; có thể tạo tài khoản riêng bằng **MỞ WEBSITE**. Không bắt buộc mọi người cùng dùng tài khoản mẫu.
5. Khi nghỉ: thoát Client → **DỪNG AN TOÀN** → đợi hoàn tất rồi mới tắt máy. Đóng Launcher không tự tắt Server.

Không chạy đồng thời với GameServer WSL2/VMware khác. Bản này không yêu cầu xóa WSL hiện có và không tự xóa bộ game cũ. Liones có mô hình8B; CPU có thể phản hồi chậm hơn GPU. Không tự tắt firewall/Hyper-V/VBS để thử.

## WinSCP và chỉnh file

Trong Launcher mở **WINSCP / HƯỚNG DẪN SỬA FILE** sau khi Server chạy. Nó xác định IP hiện tại, user/root, cổng22, khóa riêng và dấu vân tay đúng máy ảo. **Không dùng IP trên ảnh của người khác hoặc mật khẩu root/123456**. Hướng dẫn có cách dùng SFTP/khóa và dừng game để chỉnh file khi giữ SSH.

Không gửi private key `.ppk`, `Server_VMW/access/phase1_id`, database hay nhân vật lên GitHub/nhóm công khai. Sao lưu trước khi chỉnh file và giữ đúng bảng mã script.

## Người đã có bản cũ

Đây là bộ cài sạch riêng, **không tự chuyển nhân vật cũ**. Giữ nguyên game cũ nếu cần nhân vật; không cài đè hoặc xóa VMDK cũ để giải phóng chỗ. Sau khi bản mới chạy đạt, chỉ xóa bộ EXE/BIN đã tải nếu muốn lấy lại dung lượng, hoặc chuyển bộ tải ra ổ ngoài. Không xóa thư mục game đã cài.

## Phạm vi kiểm thử và báo lỗi

Đã kiểm thử cài mới trong đường dẫn có dấu, đủ SHA8.474file, active loop, AI/IPC/knowledge, website MEL, SSH, Start lặp và Stop sạch trên máy dựng. **Chưa nghiệm thu đăng nhập/đi map/chơi trên mọi máy người dùng của bản Lite này.** Đọc `KIEM_THU.txt` để thử nhân vật, map/chat/F3/TốngKim/thú cưỡi và đăng nhập lại.

Nếu gặp lỗi: gửi thông báo, bước thao tác, cấu hình Windows/VMware và log đã loại thông tin riêng tư. Không xóa WSL/VM/database hoặc force power off để thử. Kho này chỉ chứa tài liệu và bộ phát hành đã đóng gói; không chứa nguồn game, dữ liệu QA hay khóa máy người dựng. Giấy phép thành phần bên thứ ba nằm trong fileZIP đi kèm.
