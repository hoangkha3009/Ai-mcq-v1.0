# Video AI Question Generator

Ứng dụng chuyển đổi video thành câu hỏi trắc nghiệm sử dụng Whisper và Gemini AI.

## Cấu trúc thư mục

```
VideoAIApp/
├── bin/                    # Chứa các file thực thi ffmpeg
├── config/                 # Chứa file cấu hình và system prompt
├── models/                 # Chứa model Whisper
├── main.py                # File chính của ứng dụng
├── requirements.txt       # Các thư viện cần thiết
└── README.md             # Hướng dẫn sử dụng
```

## Cài đặt

1. Cài đặt Python 3.8 trở lên
2. Cài đặt các thư viện cần thiết:
   ```bash
   pip install -r requirements.txt
   ```
3. Tải và cài đặt Whisper:
   ```bash
   pip install openai-whisper
   ```
4. Copy các file ffmpeg vào thư mục bin:
   - ffmpeg.exe
   - ffprobe.exe

## Sử dụng

1. Chạy ứng dụng:
   ```bash
   python main.py
   ```
2. Chọn video cần xử lý
3. Nhấn "Transcribe" để chuyển đổi video thành text
4. Nhấn "Generate Questions" để tạo câu hỏi trắc nghiệm

## Lưu ý

- Đảm bảo đã cài đặt đầy đủ các thư viện và công cụ cần thiết
- API key Gemini đã được cấu hình trong file config.py
- Model Whisper medium sẽ được tải tự động khi chạy lần đầu 
