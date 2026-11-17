# **BÀI TẬP: SỬA ĐỔI PROMPT THIẾU CẤU TRÚC RÀNG BUỘC ĐỊNH DẠNG**

## **1. Phân tích lỗi**

Prompt cũ: “Hãy giải thích ngắn gọn các nội dung của Chain-of-Thought, Prompt Chaining, xử lý đứt gãy.”

**Ba phần văn bản thừa thãi thường xuất hiện:**

1. Lời chào: “Xin chào! Rất vui được hỗ trợ bạn.”
2. Lời dẫn: “Trước tiên, chúng ta hãy cùng tìm hiểu về chủ đề này.”
3. Lời kết: “Hy vọng những thông tin trên sẽ giúp ích cho bạn!”

**Nguyên nhân:** Prompt chưa quy định cấu trúc đầu ra, chưa giới hạn nội dung và chưa cấm lời chào, lời kết nên AI dễ tạo văn bản dài dòng.

## **2. Prompt đã tối ưu**

```
Hãy giải thích 3 nội dung:
1. Chain-of-Thought.
2. Prompt Chaining.
3. Xử lý đứt gãy ngữ cảnh.

Yêu cầu bắt buộc:
- Trình bày bằng gạch đầu dòng.
- Mỗi nội dung tối đa 2 câu.
- Sử dụng ngôn ngữ đơn giản, dễ hiểu.
- Không viết lời chào hoặc lời dẫn ở đầu.
- Không viết lời kết hoặc nội dung ngoài yêu cầu.
- Chỉ trả về nội dung kiến thức.
```

## **3. Kết quả phản hồi của AI**

- **Chain-of-Thought:** Kỹ thuật giúp AI phân tích vấn đề qua các bước logic trước khi đưa ra câu trả lời.
- **Prompt Chaining:** Kỹ thuật chia nhiệm vụ lớn thành nhiều prompt nhỏ, kết quả bước trước được dùng làm đầu vào cho bước sau.
- **Xử lý đứt gãy ngữ cảnh:** Duy trì và chuyển giao thông tin quan trọng giữa các lượt hội thoại để AI không mất bối cảnh.
