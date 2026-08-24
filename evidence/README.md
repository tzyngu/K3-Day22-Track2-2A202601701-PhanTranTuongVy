# Phân tích kết quả Day 22

## So sánh Prompt V1 và V2

Prompt V1 đạt faithfulness `0.9538` và answer relevancy `0.9201`, cao hơn
Prompt V2 với faithfulness `0.8333` và answer relevancy `0.8993`. Vì vậy,
Prompt V1 phù hợp hơn cho hệ thống RAG này: câu trả lời ngắn gọn giúp mô hình
bám sát context và trực tiếp hơn với câu hỏi.

Hai phiên bản đều đạt context recall `1.0000` và context precision khoảng
`0.9417`. Điều này cho thấy chất lượng truy xuất gần như không thay đổi giữa
hai phiên bản; khác biệt điểm số chủ yếu đến từ cách prompt hướng dẫn LLM tạo
câu trả lời.

## Kết luận

Cả V1 và V2 đều vượt mục tiêu faithfulness tối thiểu `0.8`, nhưng V1 là phiên
bản được ưu tiên dựa trên kết quả đánh giá tổng thể.
