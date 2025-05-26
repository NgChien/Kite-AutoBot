# Kite-AutoBot
Complete 10 Stars And I Will Upload kiteAi Testnet Script
# GoKiteAI V2 Bot

## Giới thiệu

GoKiteAI V2 Bot là một công cụ tự động hóa các tác vụ trên nền tảng GoKite, hỗ trợ nhiều tài khoản cùng lúc, giúp người dùng tối ưu hóa việc tích điểm, làm quiz, mint badges, staking, và tương tác với agent AI. Bot được cấu hình linh hoạt qua file `config.js` mà không cần sửa code chính.

## Tính năng chính

- **Tự động làm Daily Quiz** để nhận điểm XP mỗi ngày.
- **Mint Badges** tự động (nếu bật).
- **Tự động chat với agent AI** để giữ tài khoản luôn hoạt động (nếu bật).
- **Tự động làm Quiz Onboard** cho tài khoản mới (nếu bật).
- **Tự động Stake/Undelegate** (nếu bật).
- Hỗ trợ chạy song song nhiều tài khoản với proxy ngẫu nhiên.
- Giao diện console trực quan, báo cáo trạng thái từng tài khoản.

## Cấu trúc thư mục

- `index.js`: File khởi động chính của bot.
- `config.js`: File cấu hình các chức năng bot.
- `accounts.txt`: Danh sách private key của các tài khoản (mỗi dòng 1 private key).
- `main/`, `utils/`: Chứa mã nguồn chính và các tiện ích hỗ trợ.
- `Run.bat`: Script chạy nhanh cho Windows.
- `package.json`: Thông tin và dependencies của dự án.

## Hướng dẫn cài đặt

1. **Cài Node.js** (khuyến nghị Node 16+).
2. **Cài dependencies**:
   ```
   npm install
   ```
3. **Chuẩn bị file `accounts.txt`**  
   - Mỗi dòng là một private key của tài khoản ví 

4. **Cấu hình bot**  
   - Mở file `config.js` để bật/tắt các chức năng như Mint Badges, Daily Quiz, Chat Agent, Stake, số lượng tài khoản chạy song song (`CONCURRENCY`),...

## Hướng dẫn sử dụng

- **Chạy bot trên Windows**:  
  Nhấp đúp vào file `Run.bat` hoặc chạy lệnh:
  ```
  node index.js
  ```
- **Theo dõi kết quả**:  
  Kết quả sẽ hiển thị trực tiếp trên console, bao gồm điểm XP, trạng thái chat, proxy sử dụng, v.v.

## Lưu ý bảo mật

- **Không chia sẻ file `accounts.txt`** hoặc private key cho bất kỳ ai.
- Sử dụng proxy để bảo vệ danh tính và tránh bị giới hạn IP.

## Dependencies chính

- axios, ethers, chalk, figlet, ora, moment-timezone, random-useragent, p-limit, https-proxy-agent, socks-proxy-agent, user-agents, dotenv, async-lock, eventsource-parser, jwt-decode

## Đóng góp & liên hệ

- Đóng góp code hoặc báo lỗi qua Github hoặc liên hệ trực tiếp với tác giả. 
