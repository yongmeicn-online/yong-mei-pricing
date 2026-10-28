YONG MEI PRICING – GÓI WEB APP (PWA)

Mục tiêu:
- Dùng chung một địa chỉ trên máy tính và iPhone.
- Có thể thêm icon YM Pricing lên màn hình chính iPhone.
- Có bộ nhớ đệm cơ bản để mở lại ứng dụng khi mạng chập chờn sau lần truy cập đầu tiên.

CẤU TRÚC
- index.html: ứng dụng tính giá (giữ nguyên phần công thức từ bản iPhone đã chỉnh giao diện).
- manifest.webmanifest: tên, màu và icon ứng dụng.
- sw.js: bộ nhớ đệm ứng dụng.
- icons/: biểu tượng Yong Mei.

CÁCH TRIỂN KHAI DỄ NHẤT: GITHUB PAGES
1. Đăng nhập hoặc tạo tài khoản GitHub.
2. Tạo repository mới, ví dụ: yong-mei-pricing. Nếu đây là công cụ nội bộ, hãy nhớ rằng website GitHub Pages thường là công khai; không tải dữ liệu nhạy cảm lên repository công khai.
3. Tải TOÀN BỘ nội dung trong thư mục này lên thư mục gốc repository, không chỉ tải file ZIP.
4. Vào Settings > Pages.
5. Trong Build and deployment, chọn Deploy from a branch; Branch: main; Folder: /(root), rồi Save.
6. Chờ GitHub cấp địa chỉ HTTPS dạng https://TEN-TAI-KHOAN.github.io/yong-mei-pricing/.
7. Mở địa chỉ đó trên máy tính để kiểm tra, rồi mở cùng địa chỉ bằng Safari trên iPhone.
8. Trên iPhone: Safari > Chia sẻ > Thêm vào màn hình chính. Nếu có tùy chọn “Mở dưới dạng ứng dụng web”, bật tùy chọn đó rồi nhấn Thêm.

LƯU Ý QUAN TRỌNG
- Mọi máy dùng cùng phiên bản ứng dụng qua cùng URL, nhưng dữ liệu lưu bằng localStorage trên trình duyệt thường không tự đồng bộ giữa iPhone và máy tính. Nếu cần đồng bộ thư viện vật liệu/cấu hình hoặc báo giá giữa các thiết bị, cần bổ sung cơ sở dữ liệu hoặc dịch vụ đăng nhập/lưu trữ chung.
- Gói này không tự triển khai lên internet. Anh cần thực hiện bước hosting ở trên hoặc dùng một hosting HTTPS khác.
- Nếu thông tin báo giá là nội bộ, hãy chọn hosting/repository riêng tư phù hợp và kiểm tra chính sách truy cập trước khi đưa dữ liệu thật lên.
