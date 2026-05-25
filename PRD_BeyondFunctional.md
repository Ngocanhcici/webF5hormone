# PRD – Product Requirements Document
## Website: BeyondFunctional.vn
**Phiên bản:** 1.0  
**Ngày:** 23/05/2026  
**Người phân tích:** Claude (dựa trên reverse engineering website hiện tại)  
**Trạng thái:** Draft

---

## 1. Tổng quan sản phẩm

### 1.1 Mô tả
BeyondFunctional.vn là website cá nhân thương hiệu của Huyền Lưu – Cố vấn Sức khỏe Chức năng (Functional Health Advisor). Website phục vụ đồng thời ba mục đích: **marketing cá nhân**, **bán khóa học online**, và **đặt lịch tư vấn 1-1**.

### 1.2 Tuyên ngôn sản phẩm
> "Giúp phụ nữ tri thức hiện đại hiểu và vận hành sức khỏe một cách đơn giản, logic, thực tế và có hệ thống."

### 1.3 Nền tảng công nghệ hiện tại
- **CMS:** Wix.com Website Builder
- **Nền tảng khóa học:** Circle.so
- **Đặt lịch:** YouCanBook.me (nhúng lịch calendar)
- **Cộng đồng:** Circle.so (community riêng)
- **Email marketing:** Form đăng ký bản tin (tích hợp Wix)

---

## 2. Người dùng mục tiêu (Target Users)

### Persona chính: "Chị Hiện Đại"
| Thuộc tính | Chi tiết |
|---|---|
| Giới tính | Nữ |
| Độ tuổi | 28 – 45 |
| Nghề nghiệp | Văn phòng, chuyên môn, kinh doanh |
| Thu nhập | Trung – khá (đủ chi trả 2–4 triệu/khóa học) |
| Vấn đề sức khỏe | Mệt mỏi mãn tính, rối loạn nội tiết, khó giảm cân, mất ngủ, rối loạn tiêu hóa |
| Hành vi | Đọc nhiều, theo dõi KOL sức khỏe, đã thử nhiều phương pháp nhưng chưa hiệu quả |
| Nỗi đau cốt lõi | "Đi khám bác sĩ bảo bình thường nhưng vẫn không khỏe" |

### Persona phụ: "Người quan tâm gia đình"
Người muốn chủ động chăm sóc sức khỏe cho gia đình dựa trên kiến thức, không phụ thuộc quảng cáo TPCN.

---

## 3. Mục tiêu kinh doanh & KPIs

| Mục tiêu | KPI gợi ý |
|---|---|
| Tăng nhận biết thương hiệu | Lượt truy cập website, follower mạng xã hội |
| Chuyển đổi học viên | Tỉ lệ đăng ký khóa học / lượt xem trang khóa học |
| Booking tư vấn 1-1 | Số lịch đặt mỗi tháng |
| Xây dựng cộng đồng | Thành viên trên Circle |
| Lead generation | Email subscribers (bản tin) |
| Tải HVCO (mồi) | Số lượt download checklist xét nghiệm máu |

---

## 4. Cấu trúc website (Information Architecture)

```
beyondfunctional.vn/
├── / (Trang chủ)
│   ├── Hero section – giới thiệu + tagline
│   ├── Functional Health là gì?
│   ├── Huyền giúp bạn như thế nào? (4 trụ cột)
│   ├── Các vấn đề sức khỏe được hỗ trợ
│   ├── Sự khác biệt cốt lõi (triết lý)
│   ├── About Me – credentials
│   ├── Bắt đầu từ đâu (CTA: cộng đồng Circle & checklist)
│   ├── Khóa học nổi bật (Combo Rebalance 360)
│   ├── Coaching 1-1 + Booking lịch
│   ├── Testimonials (dạng gallery ảnh)
│   └── Blog mới nhất (3 bài)
│
├── /khoa-hoc (Trang khóa học)
│   ├── Khóa 1: Cân bằng Nội tiết – 2.495.000đ
│   ├── Khóa 2: Dinh dưỡng & TPCN Thông minh – 2.250.000đ
│   ├── Khóa 3: Stress, Detox, Giấc ngủ & Phục hồi – 1.650.000đ
│   ├── Combo ReBALANCE 360 – 4.100.000đ (giảm 35%)
│   ├── Phương thức học (Circle, Zalo, Live Q&A)
│   └── Testimonials
│
├── /blog (Blog)
│   └── Danh sách bài viết theo chuyên mục
│
├── /event-list (Sự kiện)
│
├── /community-invitation (Tham gia cộng đồng Circle)
│
└── /checklist-fbca (Landing page tải checklist)
```

---

## 5. Tính năng chi tiết (Feature Specifications)

### 5.1 Trang chủ

#### Hero Section
- **Mô tả:** Banner chính với tagline "Tôi không bị bệnh, nhưng rõ ràng không khỏe! Đi tìm nguyên nhân ngay"
- **Thành phần:** Ảnh Huyền Lưu, tên + chức danh, mô tả ngắn, navigation bar
- **CTA:** Ngầm định – kéo người dùng scroll tiếp

#### Giáo dục thương hiệu (Brand Education)
- Giải thích "Functional Health là gì?" theo cách dễ hiểu
- 4 cột nội dung: Hiểu gốc rễ / Cá nhân hóa / 4 trụ cột / Khai vấn đồng hành
- Visual storytelling với icon/ảnh minh họa

#### Social Proof – Testimonials
- **Định dạng:** Gallery ảnh screenshot phản hồi học viên
- **Số lượng:** 19+ testimonials, có nút "Xem thêm"
- **Vấn đề hiện tại:** Testimonials dạng ảnh (không có text thuần), khó index SEO

#### Booking 1-1 (Nhúng lịch)
- Calendar chọn ngày/giờ tư vấn trực tuyến
- Múi giờ UTC hiện tại (cần cá nhân hóa theo múi giờ Việt Nam)
- Tích hợp qua YouCanBook.me

#### Blog Preview
- Hiển thị 3 bài mới nhất
- Thumbnail, tiêu đề, chuyên mục, ngày đăng, thời gian đọc

---

### 5.2 Trang khóa học

#### Listing 3 khóa học đơn
| Khóa | Nội dung chính | Giá | Trạng thái |
|---|---|---|---|
| Cân bằng Nội tiết | Hormone nữ, tuyến giáp, PCOS, xét nghiệm | 2.495.000đ | Đã mở |
| Dinh dưỡng & TPCN Thông minh | Macro, tiêu hóa, vi chất, đọc nhãn, AI | 2.250.000đ | Mở từ 12/8 |
| Stress, Detox, Giấc ngủ & Phục hồi | HPA, detox gan/ruột, nhịp sinh học | 1.650.000đ | Cuối tháng 8 |

#### Combo ReBALANCE 360
- Gói 3-in-1: 4.100.000đ (tiết kiệm 35% so với mua lẻ pre-order)
- Giá gốc pre-order: 6.350.000đ
- Nhấn mạnh tư duy hệ thống thay vì học rời rạc

#### Phương thức học
- Video on-demand trên Circle (có app mobile)
- Tài liệu khóa học đi kèm
- Quyền truy cập 1 năm
- Nhóm Zalo hỗ trợ học viên
- Live Q&A 1 lần/tháng

---

### 5.3 Blog

- Hệ thống bài viết theo chuyên mục (ví dụ: "Thực phẩm chức năng")
- Thể hiện chuyên môn, hỗ trợ SEO organic
- Bài viết hiện tại tập trung vào chủ đề TPCN, dinh dưỡng, hormone

---

### 5.4 Lead Magnets & Conversion Assets

| Asset | Mô tả | CTA |
|---|---|---|
| Checklist xét nghiệm máu FBCA | Tài liệu miễn phí tải về | "Download Checklist" |
| Tham gia cộng đồng Circle | Q&A, workshop, bài viết chuyên sâu | "Tham gia ngay" |
| Đăng ký bản tin email | Form đơn giản, yêu cầu checkbox đồng ý | Nút "Xác nhận" |

---

## 6. Phân tích Gap & Điểm cần cải thiện

### 6.1 UX/UI
| Vấn đề | Mức độ | Đề xuất |
|---|---|---|
| Testimonials là ảnh chụp màn hình, không có text | Cao | Thêm dạng text card có trích dẫn để SEO và accessibility |
| Booking lịch hiển thị múi giờ UTC | Trung bình | Tự động detect múi giờ người dùng hoặc hiển thị GMT+7 |
| Không có trang giới thiệu riêng (About page) | Trung bình | Tách section "About" thành trang độc lập |
| CTA chính của Hero section không rõ | Cao | Thêm nút CTA nổi bật (vd: "Khám phá khóa học" hoặc "Book tư vấn") |
| Social icons footer trỏ về Wix mặc định (Facebook/Twitter/Instagram của Wix) | Cao | Cập nhật đúng link fanpage Huyền Lưu |

### 6.2 SEO & Content
| Vấn đề | Mức độ | Đề xuất |
|---|---|---|
| Meta description chưa tối ưu | Trung bình | Viết meta description cho từng trang |
| Blog cần đẩy thêm nội dung thường xuyên | Cao | Lịch đăng bài ít nhất 2 bài/tuần |
| Không có structured data (schema.org) | Trung bình | Thêm Schema cho Course, Person, FAQ |

### 6.3 Chuyển đổi (Conversion)
| Vấn đề | Mức độ | Đề xuất |
|---|---|---|
| Không có trang landing page riêng cho từng khóa học | Cao | Mỗi khóa cần 1 sales page dài, có FAQ và đảm bảo hoàn tiền |
| Không hiển thị số học viên hoặc kết quả cụ thể | Trung bình | Thêm số liệu xã hội (vd: "500+ học viên") |
| Không có chính sách hoàn tiền rõ ràng | Trung bình | Thêm hoàn tiền 7-14 ngày để giảm rủi ro cho người mua |
| Email opt-in form đơn giản, không có HVCO kèm theo | Trung bình | Cung cấp lead magnet kèm theo khi đăng ký email |

### 6.4 Kỹ thuật
| Vấn đề | Mức độ | Đề xuất |
|---|---|---|
| Website build trên Wix – giới hạn customization và tốc độ | Thấp | Xem xét migrate sang Next.js/Webflow trong dài hạn |
| Không có tracking rõ ràng (GA4, Pixel) | Cao | Cài Google Analytics 4 + Meta Pixel để đo conversion |
| Không có live chat / chatbot | Thấp | Thêm Zalo Chat widget hoặc Facebook Messenger plugin |

---

## 7. Luồng người dùng chính (User Flows)

### Flow 1: Khách lạ → Mua khóa học
```
Tìm kiếm Google / thấy Facebook post
→ Landing trang chủ
→ Đọc "Functional Health là gì?"
→ Nhận ra triệu chứng của mình
→ Xem khóa học → Chọn Combo ReBALANCE 360
→ Đăng ký → Thanh toán → Học trên Circle
```

### Flow 2: Khách lạ → Download checklist → Email nurture
```
Thấy post Facebook/YouTube
→ Landing trang checklist FBCA
→ Điền email → Nhận checklist
→ Nhận bản tin → Chuyển đổi mua khóa học
```

### Flow 3: Khách có vấn đề nghiêm trọng → Booking 1-1
```
Tìm kiếm thông tin về bệnh cụ thể (Hashimoto, PCOS...)
→ Blog post chuyên sâu
→ CTA booking tư vấn
→ Chọn lịch → Điền form → Xác nhận lịch hẹn
```

---

## 8. Nội dung ưu tiên (Content Priorities)

| Chuyên mục | Ưu tiên | Lý do |
|---|---|---|
| Hormone nữ / Nội tiết | Cao | Core offer, pain point lớn nhất |
| Tuyến giáp (Hashimoto, suy giáp) | Cao | Từ khóa tìm kiếm cao |
| Tiêu hóa (IBS, SIBO) | Trung bình | Nhóm khách hàng rộng |
| Dinh dưỡng thực hành | Trung bình | SEO organic tốt |
| TPCN & supplement | Cao | Xu hướng thị trường, dễ viral |
| Xét nghiệm máu / FBCA | Cao | Differentiator độc đáo |

---

## 9. Lộ trình phát triển đề xuất (Roadmap)

### Phase 1 – Quick Wins (0–4 tuần)
- Sửa social links footer trỏ đúng fanpage
- Thêm CTA nút rõ ràng vào Hero section
- Cài Google Analytics 4 + Meta Pixel
- Thêm FAQ section trên trang khóa học
- Hiển thị múi giờ GMT+7 cho booking lịch

### Phase 2 – Tăng chuyển đổi (1–3 tháng)
- Tạo sales page riêng cho từng khóa học
- Chuyển testimonials từ ảnh sang dạng text card
- Thêm chính sách hoàn tiền
- Thêm số học viên / kết quả cụ thể
- Xây dựng email sequence tự động sau khi opt-in

### Phase 3 – Mở rộng (3–6 tháng)
- Thêm trang About riêng với timeline & credentails đầy đủ
- Ra mắt chương trình affiliate / refer học viên
- Tích hợp livestream / sự kiện trực tuyến
- Xây dựng App hoặc tối ưu trải nghiệm mobile

---

## 10. Hệ thống pricing hiện tại

| Sản phẩm | Giá | Hình thức |
|---|---|---|
| Khóa Cân bằng Nội tiết | 2.495.000đ | Pre-order, học ngay |
| Khóa Dinh dưỡng & TPCN | 2.250.000đ | Pre-order, mở 12/8 |
| Khóa Stress & Phục hồi | 1.650.000đ | Pre-order, mở cuối tháng 8 |
| Combo ReBALANCE 360 | 4.100.000đ | Bundle 3 khóa, tiết kiệm 35% |
| Coaching 1-1 | Theo thỏa thuận | Đặt lịch qua YouCanBook.me |

---

## 11. Integrations hiện tại

| Hệ thống | Mục đích | Trạng thái |
|---|---|---|
| Wix | CMS & hosting | Đang dùng |
| Circle.so | Khóa học & cộng đồng | Đang dùng |
| YouCanBook.me | Booking lịch tư vấn | Đang dùng |
| Facebook | Marketing & traffic chính | Đang dùng |
| YouTube | Content video | Đang dùng |
| Zalo | Support học viên (trợ lý Linh Lê) | Đang dùng |
| Email (Gmail) | Liên hệ & hỗ trợ | trolyhuyenluu@gmail.com |

---

*Document này được tạo dựa trên phân tích công khai website beyondfunctional.vn tại thời điểm 23/05/2026.*
