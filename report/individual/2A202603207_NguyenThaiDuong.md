# Báo cáo thực hành Day 3

- Mã học viên theo lớp: 2A202603207
- Ngày / CVAT: 12/11/2026 / CVAT online (app.cvat.ai) – không chạy được CVAT local
- Công cụ đã dùng: Polygon
## 1. Bài đã nộp

| Task | File ZIP đúng tên | Hoàn thành mấy ảnh | Điểm tối đa (coach chấm sau) |
| --- | --- | ---: | ---: |
| easy_semantic | easy_semantic.zip | 3 / 3 | 20 |
| medium_instance | medium_instance.zip | 3 / 3 | 32 |
| hard_panoptic | hard_panoptic.zip | [2] / 2 | 30 |
| cp1_holes | chưa có | 0 / 1 | 3 |
| cp2_slice | chưa có | 0 / 1 | 3 |
| cp5_occlusion | chưa có | 0 / 1 | 3 |
| cp3_thin | chưa có | 0 / 1 | 3 |
| cp4_curb | chưa có | 0 / 1 | 3 |
| cp6_coverage | chưa có | 0 / 1 | 3 |
| **Tổng tối đa** | | | **100** |

Sáu checkpoint chưa kịp làm do hết thời gian và tài khoản CVAT miễn phí báo giới hạn số task. Lần export Medium đầu bị nhầm format CVAT XML, đã export lại COCO 1.0.

## 2. Một quyết định trước khi dùng gợi ý

- Ảnh, vị trí và object Medium đầu tiên tự vẽ: 000000181542, ở giữa ảnh, người áo trắng
- Class và quy tắc tôi dùng để chọn biên: person, sử dụng xung quanh người
- Nếu dùng gợi ý sau đó: 

## 3. Một lỗi tôi tìm thấy và sửa

- Task/ảnh/vùng: hard_panoptic / 000000460147.jpg / xe lớn giữa đường chở ô tô con
- Lỗi thuộc loại: sai lớp
- Bằng chứng tôi nhìn thấy: Do xe có 2 tầng và chở ô tô con trong xe
- Quy tắc và hành động sửa: đổi bus → truck, vì xe bus không như thế nên xe đó là xe tải 
- Sau sửa đã Save và export lại chưa? Rồi

## 4. Ba ca chưa chắc hoặc đã cân nhắc

| Ảnh/vị trí | Hai cách hiểu có thể | Quy tắc/chứng cứ | Quyết định hoặc câu hỏi cho coach |
| --- | --- | --- | --- |
| easy 7ee6d192, sườn đồi cỏ khô hai bên | [...] | [...] | [...] |
| hard 000000460147, đoàn xe nhỏ dày đặc ở xa | [...] | [...] | [...] |
| hard 000000460147, ô tô nằm trên xe tải chở xe | [...] | [...] | [...] |
