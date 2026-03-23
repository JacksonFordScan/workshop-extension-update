Cách Update Extension
Bước 1: Sửa Version trong code
Mở file manifest.json trong thư mục code gốc, tăng số phiên bản lên.
(Ví dụ: đang là "2.0.0" thì sửa thành "2.0.1").

Bước 2: Pack lại ra file CRX

Mở chrome://extensions/ -> Bấm Pack extension.

Extension root directory: Chọn thư mục code vừa sửa.

Private key file (Bắt buộc): Chọn cái file .pem cũ

Đổi tên file .crx vừa sinh ra thành đúng tên workshop-tool.crx.

Bước 3: Cập nhật file XML
Mở file update.xml, sửa chỗ version='2.0.0' thành phiên bản mới trùng với Bước 1 (ví dụ: version='2.0.1'). Giữ nguyên cái link tải.

Bước 4: Đẩy lên Server (GitHub)
Copy 2 file ford-extension.crx và update.xml vừa làm xong, push đè (commit) lên nhánh main của repo incode-workshop-extention-git trên GitHub.