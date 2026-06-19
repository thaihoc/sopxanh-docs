# Đề xuất Lộ trình Chuyển đổi số cho GODACO Seafood

> Tài liệu đề xuất lộ trình chuyển đổi số (CĐS) theo từng giai đoạn cho GODACO Seafood, xây dựng trên đặc thù mô hình **tích hợp dọc** (vùng nuôi → nhà máy thức ăn → chế biến → kho lạnh → xuất khẩu) và định hướng đã nêu trong [Bản đồ ánh xạ Nhu cầu – Giải pháp](./ban-do-anh-xa-giai-phap-godaco.md).
>
> Định hướng giải pháp ở mức tổng quát, trung lập về nhà cung cấp; tên sản phẩm – dịch vụ cụ thể sẽ chốt theo giai đoạn triển khai thực tế.

---

## 1. Bối cảnh và căn cứ đề xuất

GODACO Seafood là doanh nghiệp thủy sản tích hợp dọc với hơn 28 năm kinh nghiệm, tự cung ứng 100%, sản lượng hơn 100.000 tấn/năm, 8 nhà máy chế biến (mới nhất là Trúc Giang – EU Code TS 1306), vùng nuôi 300 ha (hơn 80 ha đạt ASC), sản phẩm có mặt tại 120+ quốc gia và sở hữu hàng loạt chứng nhận quốc tế (ASC, MSC, BAP, BRC, IFS, HACCP, Halal, ISO 17025, BSCI, SA 8000...).

Những đặc điểm này định hình **bốn áp lực chuyển đổi số cốt lõi**:

1. **Áp lực tuân thủ & truy xuất nguồn gốc** — thị trường EU/Mỹ/Nhật yêu cầu truy xuất farm-to-fork, chống IUU, sẵn sàng EUDR và báo cáo ESG. Đây là yếu tố *sống còn* với năng lực xuất khẩu.
2. **Áp lực vận hành đa điểm** — 8 nhà máy + nhiều vùng nuôi phân tán cần dữ liệu thống nhất, thời gian thực.
3. **Áp lực kiểm soát chất lượng & chi phí** — yield, OEE, FCR, chuỗi lạnh ảnh hưởng trực tiếp biên lợi nhuận.
4. **Áp lực cạnh tranh & bền vững** — định vị thương hiệu "Sustainability" cần được chứng minh bằng dữ liệu.

### Nguyên tắc thiết kế lộ trình

- **ERP là trục xương sống:** triển khai sớm vì mọi hệ thống khác cần "cắm" dữ liệu vào.
- **Ưu tiên ROI và rủi ro xuất khẩu:** truy xuất nguồn gốc và quản lý chất lượng được đẩy sớm vì bảo vệ trực tiếp doanh thu xuất khẩu.
- **Tránh dàn trải:** mỗi giai đoạn có trọng tâm rõ, hoàn thành nền tảng trước khi mở rộng.
- **Đo lường được:** mỗi giai đoạn gắn KPI nghiệm thu cụ thể.

---

## 2. Tổng quan lộ trình 4 giai đoạn

| Giai đoạn | Tên | Thời gian dự kiến | Trọng tâm | Kết quả then chốt |
|---|---|---|---|---|
| **GĐ 0** | Khởi động & Đánh giá | 1–3 tháng | Kiểm toán hiện trạng, quản trị CĐS, lộ trình chi tiết | Bản đồ hệ thống hiện trạng + kế hoạch chốt |
| **GĐ 1** | Nền móng số | 6–12 tháng | Hạ tầng, ATTT, Chữ ký số, **ERP** (TC-KT, Mua hàng, Kho, SX, Bán hàng), **HRM–Chấm công–Tiền lương**, Quản lý tài sản, Quản lý dự án, Hóa đơn/Hợp đồng điện tử | Trục dữ liệu & quản trị nội bộ vận hành |
| **GĐ 2** | Vận hành chuyên sâu | 12–24 tháng | MES, WMS + chuỗi lạnh, **Truy xuất nguồn gốc**, QMS/LIMS, CRM/Cổng B2B | Số hóa toàn chuỗi giá trị, sẵn sàng audit |
| **GĐ 3** | Thông minh hóa | Song song & sau GĐ2 (18 tháng+) | IoT vùng nuôi, BI/IOC, AI, ESG | Ra quyết định bằng dữ liệu & dự báo |

```
GĐ0 ──► GĐ1 (Nền móng) ──────► GĐ2 (Chuyên sâu) ──► GĐ3 (Thông minh)
 │           │                       │                    │
Đánh giá   ERP + HR/Lương +      MES/WMS/TXNG +       IoT/BI/AI/ESG
           Tài sản + Dự án       QMS/LIMS/CRM
           + Hạ tầng/ATTT
```

> **Nguyên tắc xếp giai đoạn (tư vấn):** thứ tự được quyết định trước hết bởi **ràng buộc phụ thuộc** (cái nào là đầu vào của cái nào), sau đó trong cùng một lớp thì **ưu tiên giải pháp mang lại lợi thế cạnh tranh & hiệu quả kinh doanh cao nhất, chi phí/phụ thuộc thấp nhất** làm trước. Xem chi tiết ở [Mục 4 – Bản đồ phụ thuộc & ưu tiên](#4-bản-đồ-phụ-thuộc-giữa-các-hệ-thống).

---

## 3. Chi tiết từng giai đoạn

### Giai đoạn 0 — Khởi động & Đánh giá hiện trạng *(1–3 tháng)*

**Mục tiêu:** Không "đốt cháy giai đoạn". Trước khi đầu tư lớn, cần hiểu rõ hiện trạng và thiết lập bộ máy quản trị chuyển đổi số.

**Việc cần làm:**
- Kiểm toán hệ thống CNTT hiện hữu (phần mềm kế toán, file Excel, hạ tầng mạng từng nhà máy, phần mềm rời rạc đang dùng).
- Khảo sát quy trình nghiệp vụ end-to-end theo chuỗi giá trị tích hợp dọc.
- Thành lập **Ban Chỉ đạo CĐS** (lãnh đạo bảo trợ) và **đội dự án CĐS** (PMO) liên phòng ban.
- Xây dựng kiến trúc đích (target architecture) và chuẩn dữ liệu chung (mã hàng, mã lô/mẻ, mã đối tác).
- Chốt thứ tự ưu tiên, ngân sách và tiêu chí lựa chọn nhà cung cấp.

**Giải pháp/đầu ra:** Báo cáo đánh giá hiện trạng; Kiến trúc tổng thể (enterprise architecture); Khung quản trị dữ liệu (data governance); Kế hoạch tổng thể đã được phê duyệt.

**KPI nghiệm thu:** 100% nhà máy/vùng nuôi được lập bản đồ hệ thống; danh mục dữ liệu chuẩn được phê duyệt; lộ trình & ngân sách được ký duyệt.

---

### Giai đoạn 1 — Nền móng số *(6–12 tháng)*

**Mục tiêu:** Dựng "đường ray" hạ tầng – an ninh – dữ liệu, đưa **ERP** vào vận hành làm trục xương sống, đồng thời số hóa **khối quản trị nội bộ** (nhân sự – lương – tài sản – dự án) chạy song song vì ROI nhanh và ít phụ thuộc hệ thống khác.

GĐ1 được tổ chức thành **4 luồng**, xếp theo ràng buộc phụ thuộc và ưu tiên giá trị:

#### Luồng A — Nền tảng kỹ thuật *(điều kiện tiên quyết, làm trước nhất)*

| Giải pháp | Vì sao bắt buộc trước | Phụ thuộc |
|---|---|---|
| Hạ tầng Cloud/Hybrid + SD-WAN | Mọi hệ thống cần nền chạy ổn định, đồng bộ realtime giữa 8 nhà máy | — |
| An toàn thông tin (endpoint, backup, SOC) | Sự cố ransomware có thể dừng nhà máy & mất dữ liệu truy xuất → rủi ro chí mạng | Hạ tầng |
| Chữ ký số / chứng thực điện tử | Nền pháp lý cho hóa đơn/hợp đồng/chứng từ điện tử | Hạ tầng |

#### Luồng B — Trục ERP *(xương sống, ưu tiên cao nhất)*

Triển khai **tuần tự theo dòng dữ liệu**, không làm song song toàn bộ:

```
Tài chính – Kế toán (gốc)
        │
   ┌────┴────┐
 Mua hàng   Bán hàng
   │            │
  Kho ──────► Sản xuất (lập kế hoạch)
```

| Thứ tự | Phân hệ ERP | Lý do xếp thứ tự |
|---|---|---|
| 1 | **Tài chính – Kế toán** | Gốc của mọi dòng tiền; mua hàng/bán hàng/lương/tài sản đều hạch toán về đây |
| 2 | **Quản lý mua hàng** | Tạo công nợ phải trả (đổ về kế toán) + nhập kho |
| 3 | **Quản lý kho** (inventory cơ bản) | Master hàng hóa & tồn kho là đầu vào của sản xuất; *(WMS nâng cao + chuỗi lạnh → GĐ2)* |
| 4 | **Quản lý sản xuất** (lập kế hoạch, BOM) | Cần master hàng + tồn kho; *(điều hành chi tiết MES → GĐ2)* |
| 5 | **Quản lý bán hàng (Sales)** | Tạo công nợ phải thu; *(CRM + cổng B2B → GĐ2)* |

> **Lưu ý phạm vi:** *Kho, Sản xuất, Sales* ở GĐ1 là **phân hệ lõi trong ERP**. Các bản nâng cao chuyên ngành — **WMS+IoT chuỗi lạnh, MES, CRM/Cổng B2B** — thuộc GĐ2 vì phải cắm trên trục ERP đã ổn định.

#### Luồng C — Quản trị nhân sự *(chạy song song ERP — ROI nhanh, ít phụ thuộc)*

Chuỗi phụ thuộc cứng: **HRM → Chấm công → Tiền lương**.

| Thứ tự | Giải pháp | Lý do xếp thứ tự & giá trị |
|---|---|---|
| 1 | **Phần mềm quản lý nhân sự (HRM)** | Hồ sơ nhân sự là master cho chấm công & lương; nền của cả luồng |
| 2 | **Chấm công nhận diện khuôn mặt** | Cần danh sách nhân sự từ HRM; *quick win* dễ thấy, chống gian lận công cho hàng nghìn lao động/8 nhà máy |
| 3 | **Quản lý tiền lương (Payroll)** | Cần hồ sơ HRM + dữ liệu công; kết quả lương hạch toán về Tài chính–Kế toán |

> Luồng này **không cần chờ ERP hoàn tất** — chỉ cần điểm tích hợp với phân hệ Tài chính–Kế toán. Đưa sớm vì hiệu quả vận hành rõ rệt (chuẩn hóa công – lương quy mô lớn).

#### Luồng D — Công cụ quản trị bổ trợ

| Giải pháp | Vị trí & lý do | Phụ thuộc |
|---|---|---|
| **Quản lý tài sản** | Cuối GĐ1: lập sổ tài sản/thiết bị, gắn khấu hao vào kế toán; là **tiền đề cho bảo trì dự đoán ở GĐ3** | Tài chính–Kế toán |
| **Quản lý dự án** | Đầu GĐ1: dùng làm công cụ điều hành chính chương trình CĐS & các dự án đầu tư nhà máy (ví dụ Mekong Delight) | Gần như độc lập |
| Hóa đơn / Hợp đồng điện tử, số hóa chứng từ | Quick win, giảm giấy tờ ngay, hỗ trợ chứng từ xuất khẩu | Chữ ký số |
| Nền tảng dữ liệu (Data Lake/DWH – khởi tạo) | Bắt đầu gom dữ liệu để phục vụ BI/AI ở GĐ3 | ERP (nguồn dữ liệu) |

**Cách tiếp cận triển khai:** ERP đi theo phân kỳ phân hệ như sơ đồ Luồng B, pilot tại 1–2 nhà máy rồi nhân rộng ra toàn bộ 8 nhà máy. Luồng C (nhân sự) và Luồng D (dự án) khởi động song song ngay từ đầu GĐ1.

**KPI nghiệm thu:** ERP go-live các phân hệ lõi; đóng sổ kế toán hợp nhất nhanh hơn X%; 100% hóa đơn điện tử; payroll tự động hóa, sai sót lương giảm; chấm công khuôn mặt phủ 100% lao động nhà máy; sổ tài sản số hóa đầy đủ; RPO/RTO sao lưu đạt mục tiêu; SD-WAN phủ toàn bộ nhà máy.

---

### Giai đoạn 2 — Vận hành chuyên sâu *(12–24 tháng)*

**Mục tiêu:** Số hóa sâu từng mắt xích sản xuất – kho – chất lượng – khách hàng, và đặc biệt **đóng vòng truy xuất nguồn gốc** để bảo vệ năng lực xuất khẩu.

**Nhóm giải pháp triển khai:**

| Hạng mục | Giải pháp | Giá trị mang lại |
|---|---|---|
| **Truy xuất nguồn gốc** | Nền tảng truy xuất farm-to-fork (kết hợp QR/blockchain) | **ROI nhanh** — đáp ứng EU/Mỹ/Nhật, IUU, sẵn sàng EUDR; bảo vệ trực tiếp doanh thu xuất khẩu |
| QMS + LIMS | Quản lý chất lượng & thông tin phòng lab | Sẵn sàng audit ASC, BRC, IFS, HACCP, Halal, ISO 17025; số hóa kết quả kiểm nghiệm |
| MES | Điều hành sản xuất chế biến thực phẩm | Lập lịch sản xuất, quản lý lô/mẻ, kiểm soát yield & OEE |
| WMS + IoT chuỗi lạnh | Quản lý kho theo FEFO + cảm biến nhiệt độ | Giám sát chuỗi lạnh, cảnh báo lệch nhiệt, giảm hao hụt |
| CRM + Cổng B2B | Quản lý khách hàng + cổng đặt/theo dõi đơn | Phục vụ nhập khẩu/phân phối/bán lẻ/food service tại 120+ quốc gia |

**Trình tự khuyến nghị trong GĐ2:** Truy xuất nguồn gốc + QMS/LIMS (đẩy sớm nhất vì rủi ro xuất khẩu) → MES → WMS/chuỗi lạnh → CRM/Cổng B2B. Tất cả tích hợp dữ liệu lô/mẻ và đối tác qua trục ERP.

**KPI nghiệm thu:** Truy xuất 1 lô bất kỳ < vài phút; vượt qua kỳ audit chứng nhận không lỗi lớn về hồ sơ; yield/OEE được đo realtime; tỷ lệ lệch nhiệt chuỗi lạnh giảm; % đơn hàng xuất khẩu qua cổng B2B.

---

### Giai đoạn 3 — Thông minh hóa *(triển khai song song & sau GĐ2)*

**Mục tiêu:** Khai thác kho dữ liệu đã tích lũy để dự báo, tối ưu và chứng minh phát triển bền vững — biến dữ liệu thành lợi thế cạnh tranh.

**Nhóm giải pháp triển khai:**

| Hạng mục | Giải pháp | Ứng dụng cụ thể cho GODACO |
|---|---|---|
| IoT nuôi trồng | Smart Aquaculture + cảm biến môi trường nước | Giám sát chất lượng nước, cho ăn, cảnh báo dịch bệnh, tối ưu FCR trên 300 ha |
| BI / IOC | Phân tích kinh doanh + trung tâm điều hành | KPI realtime: sản lượng, yield, tồn kho, doanh số theo thị trường |
| AI | Forecasting, computer vision, predictive maintenance | Dự báo nhu cầu/giá nguyên liệu; phân loại – phân cỡ cá; phát hiện lỗi dây chuyền; bảo trì dự đoán |
| ESG | Quản lý & báo cáo ESG | Dấu chân carbon, sử dụng nước theo yêu cầu người mua EU; tận dụng dữ liệu IoT vùng nuôi |

> **Lưu ý:** GĐ3 có thể bắt đầu song song GĐ2 với hai cấu phần nền: (1) khởi tạo data platform từ GĐ1, (2) số hóa ESG sớm để biến định vị "Sustainability" thành lợi thế bán hàng với người mua EU.

**KPI nghiệm thu:** Dashboard điều hành dùng hằng ngày bởi lãnh đạo; cải thiện FCR/giảm hao hụt nhờ IoT; độ chính xác dự báo; báo cáo ESG xuất ra theo chuẩn người mua yêu cầu.

---

## 4. Bản đồ phụ thuộc giữa các hệ thống

```
        Hạ tầng Cloud/SD-WAN + An toàn thông tin + Chữ ký số      (GĐ1 – nền kỹ thuật)
                                  │
   ┌──────────────────────────────┼───────────────────────────────┐
   │                              │                                │
 ERP (trục xương sống)        HRM ─► Chấm công ─► Tiền lương     Quản lý dự án
 TC-KT ─► Mua hàng ─► Kho          │  (Luồng C – song song)      (Luồng D – độc lập)
   └─► Sản xuất ─► Bán hàng        │
        │   │                     └──────────► (lương hạch toán về TC-KT)
        │   └─► Quản lý tài sản (cuối GĐ1, gắn khấu hao vào TC-KT)
        │                                            │
        │                                            ▼ tiền đề
   ┌────┴──────────┬──────────────┬──────────┐   (Bảo trì dự đoán – GĐ3)
  MES            WMS+IoT      Truy xuất     CRM/Cổng B2B           (GĐ2)
 (cần SX,      chuỗi lạnh    nguồn gốc      (cần Bán hàng)
  lô/mẻ)       (cần Kho)    + QMS/LIMS
        └───────────┴──────────────┴──────────┘
                          │
                Data Platform ──► BI/IOC ──► AI ──► ESG            (GĐ3)
                          ▲
                IoT (vùng nuôi + chuỗi lạnh)
```

**Nguyên tắc xếp thứ tự (đọc từ trên xuống):**

1. **Phụ thuộc trước – không triển khai lớp trên khi lớp dưới chưa ổn định.** Nền kỹ thuật → ERP → các hệ chuyên sâu (MES/WMS/CRM) → BI/AI.
2. **Trong ERP, đi theo dòng dữ liệu:** Tài chính–Kế toán là gốc, rồi Mua hàng/Bán hàng → Kho → Sản xuất.
3. **Chuỗi nhân sự là ràng buộc cứng:** HRM → Chấm công → Tiền lương; payroll nối về kế toán.
4. **Quản lý tài sản trước bảo trì dự đoán:** phải có sổ tài sản (GĐ1) mới làm predictive maintenance (GĐ3).
5. **Trong cùng một lớp, ưu tiên giá trị:** việc ít phụ thuộc + ROI/lợi thế cạnh tranh cao làm trước (HR/lương, hóa đơn điện tử ở GĐ1; truy xuất nguồn gốc + QMS/LIMS dẫn đầu GĐ2 vì bảo vệ xuất khẩu).

---

## 5. Khuyến nghị trọng điểm

1. **Hoàn thành ERP sớm và dứt điểm.** Đây là điều kiện tiên quyết; tránh triển khai nhiều hệ thống lớn cùng lúc gây quá tải nguồn lực.
2. **Chạy khối nhân sự (HRM–Chấm công–Tiền lương) song song ERP ngay trong GĐ1.** Đây là luồng ít phụ thuộc nhưng ROI nhanh, hiệu quả vận hành rõ rệt trên quy mô hàng nghìn lao động/8 nhà máy; chỉ cần một điểm tích hợp về phân hệ kế toán.
3. **Đẩy truy xuất nguồn gốc + QMS/LIMS lên ưu tiên thực tế cao** dù xếp ở GĐ2, vì chúng bảo vệ trực tiếp khả năng xuất khẩu — yếu tố sống còn.
3. **Bắt đầu thu thập dữ liệu từ GĐ1.** Data platform khởi tạo sớm để khi tới GĐ3 đã có dữ liệu lịch sử cho AI/BI.
4. **Số hóa ESG sớm** để tận dụng định vị phát triển bền vững làm lợi thế cạnh tranh với người mua EU.
5. **Quản trị thay đổi (change management).** Đầu tư đào tạo, truyền thông nội bộ và đo lường mức độ chấp nhận của người dùng — phần lớn thất bại CĐS đến từ con người, không phải công nghệ.
6. **Chọn nền tảng có khả năng tích hợp mở (API)** để các lớp cắm vào nhau dễ dàng, tránh "ốc đảo dữ liệu".

---

## 6. Yếu tố thành công và rủi ro cần quản lý

| Yếu tố thành công | Rủi ro nếu thiếu |
|---|---|
| Lãnh đạo bảo trợ, ngân sách cam kết theo lộ trình | Dự án đứt gãy giữa chừng, đầu tư lãng phí |
| Chuẩn hóa dữ liệu chung từ GĐ0 | Hệ thống không nói chuyện được với nhau |
| Triển khai theo phân kỳ, pilot trước khi nhân rộng | Go-live đồng loạt gây gián đoạn sản xuất |
| Đào tạo & quản trị thay đổi | Người dùng không dùng, hệ thống "chết lâm sàng" |
| An toàn thông tin đi cùng từ đầu | Sự cố an ninh dừng nhà máy, mất dữ liệu truy xuất |

---

## 7. Phụ lục: Giải nghĩa từ viết tắt

### Các hệ thống công nghệ
- **ERP (Enterprise Resource Planning):** Hệ thống Hoạch định tài nguyên doanh nghiệp.
- **MES (Manufacturing Execution System):** Hệ thống Điều hành sản xuất.
- **WMS (Warehouse Management System):** Hệ thống Quản lý kho.
- **QMS (Quality Management System):** Hệ thống Quản lý chất lượng.
- **LIMS (Laboratory Information Management System):** Hệ thống Quản lý thông tin phòng lab/thử nghiệm.
- **CRM (Customer Relationship Management):** Hệ thống Quản lý quan hệ khách hàng.
- **HRM (Human Resource Management):** Hệ thống Quản lý nhân sự.
- **BI (Business Intelligence):** Nền tảng Phân tích dữ liệu kinh doanh thông minh.
- **IOC (Intelligent Operations Center):** Trung tâm điều hành thông minh.
- **IoT (Internet of Things):** Internet vạn vật (các thiết bị, cảm biến được kết nối mạng).
- **SD-WAN (Software-Defined Wide Area Network):** Mạng diện rộng định nghĩa bằng phần mềm, kết nối an toàn các nhà máy/chi nhánh.
- **SOC (Security Operations Center):** Trung tâm điều hành an toàn thông tin mạng.
- **DWH (Data Warehouse):** Kho dữ liệu tập trung của doanh nghiệp.

### Các chỉ số và thuật ngữ quản trị
- **Yield:** Tỷ lệ thu hồi (sản lượng thành phẩm thu được so với nguyên liệu đầu vào).
- **OEE (Overall Equipment Effectiveness):** Hiệu suất thiết bị tổng thể (đo lường mức độ hiệu quả của dây chuyền sản xuất).
- **FCR (Feed Conversion Ratio):** Hệ số chuyển đổi thức ăn (lượng thức ăn cần thiết để tạo ra 1kg cá).
- **ROI (Return on Investment):** Tỷ suất hoàn vốn đầu tư.
- **BOM (Bill of Materials):** Định mức nguyên vật liệu sản xuất.
- **FEFO (First Expired, First Out):** Nguyên tắc xuất kho: Hàng có hạn sử dụng gần nhất phải xuất trước.
- **RPO / RTO (Recovery Point / Time Objective):** Mục tiêu điểm khôi phục / thời gian khôi phục hệ thống khi xảy ra sự cố gián đoạn.
- **PMO (Project Management Office):** Ban/Văn phòng quản lý dự án.

### Các chứng nhận và tiêu chuẩn
- **ASC, MSC, BAP:** Các tiêu chuẩn quốc tế uy tín về nuôi trồng và khai thác thủy sản bền vững.
- **BRC, IFS, HACCP:** Các tiêu chuẩn quốc tế về quản lý chất lượng và vệ sinh an toàn thực phẩm.
- **IUU (Illegal, Unreported and Unregulated fishing):** Hoạt động đánh bắt cá bất hợp pháp, không khai báo và không theo quy định.
- **EUDR (EU Deforestation Regulation):** Quy định chống phá rừng của Liên minh Châu Âu.
- **ESG (Environmental, Social, and Governance):** Khung tiêu chuẩn đo lường về Môi trường, Xã hội và Quản trị doanh nghiệp.
- **BSCI, SA 8000:** Các tiêu chuẩn về trách nhiệm xã hội trong hoạt động kinh doanh.

---

*Tài liệu đề xuất ở mức định hướng, trung lập về nhà cung cấp. Thời gian, ngân sách và tên sản phẩm – dịch vụ cụ thể sẽ được tinh chỉnh sau Giai đoạn 0 (đánh giá hiện trạng).*
