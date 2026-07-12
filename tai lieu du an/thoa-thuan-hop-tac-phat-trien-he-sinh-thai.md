# THỎA THUẬN HỢP TÁC PHÁT TRIỂN HỆ SINH THÁI PHẦN MỀM CHUYỂN ĐỔI SỐ CHO DOANH NGHIỆP

> **Phiên bản:** 1.0 (dự thảo)
> **Ngày lập:** 12/07/2026
> **Các bên tham gia:** Các thành viên có tên trong Phụ lục A — Danh sách thành viên

---

## Điều 1. Mục đích và phạm vi

1. Thỏa thuận này quy định nguyên tắc hợp tác giữa các thành viên trong việc cùng xây dựng **một bộ giải pháp hoàn chỉnh phục vụ chuyển đổi số cho doanh nghiệp** (sau đây gọi là "**Hệ sinh thái**").
2. Mỗi thành viên phụ trách phát triển một hoặc một vài giải pháp/sản phẩm trong Hệ sinh thái (sau đây gọi là "**Sản phẩm thành phần**").
3. Thỏa thuận áp dụng cho toàn bộ hoạt động: quy hoạch, phát triển, triển khai, vận hành, hỗ trợ khách hàng và bàn giao Sản phẩm thành phần.
4. Đây là hoạt động hợp tác tự nguyện, thực hiện **ngoài giờ làm việc**, bên cạnh công việc chính của các thành viên tại VNPT.

## Điều 2. Nguyên tắc hợp tác chung

1. **Tự nguyện, bình đẳng, cùng có lợi:** mọi thành viên có quyền và nghĩa vụ như nhau theo Thỏa thuận này, trừ khi có phân công vai trò cụ thể được cả nhóm thông qua.
2. **Hệ sinh thái là ưu tiên cao nhất:** lợi ích tổng thể của Hệ sinh thái được đặt trên lợi ích riêng của từng Sản phẩm thành phần.
3. **Minh bạch:** kế hoạch, tiến độ, các quyết định quan trọng và các khoản tài chính chung phải được thông báo công khai trong nhóm.
4. **Cam kết chất lượng:** sản phẩm đã triển khai cho khách hàng phải được duy trì, hỗ trợ có trách nhiệm — không bỏ rơi khách hàng trong bất kỳ hoàn cảnh nào.

## Điều 3. Tách bạch với công việc tại VNPT

1. Công việc phát triển Hệ sinh thái là **công việc làm thêm ngoài giờ**, hoàn toàn độc lập với công việc tại VNPT. Hai công việc **không được ảnh hưởng lẫn nhau**.
2. Các thành viên cam kết **KHÔNG**:
   - Dành thời gian trong giờ làm việc tại VNPT để làm công việc của Hệ sinh thái;
   - Sử dụng thiết bị, phần mềm, bản quyền, tài khoản, hạ tầng hoặc bất kỳ công cụ nào được VNPT cấp phát cho công việc của Hệ sinh thái;
   - Sử dụng source code, tài liệu, dữ liệu, thông tin nội bộ hoặc tài sản trí tuệ thuộc về VNPT trong các Sản phẩm thành phần;
   - Sử dụng danh nghĩa, thương hiệu VNPT để chào bán, quảng bá sản phẩm của Hệ sinh thái, hoặc ngược lại — gây nhầm lẫn rằng sản phẩm của Hệ sinh thái là sản phẩm của VNPT;
   - Lôi kéo khách hàng, chuyển hướng cơ hội kinh doanh thuộc về VNPT sang Hệ sinh thái.
3. Mỗi thành viên tự chịu trách nhiệm tuân thủ hợp đồng lao động, nội quy lao động và các quy định của VNPT áp dụng cho cá nhân mình. Nếu phát sinh xung đột lợi ích, thành viên phải chủ động báo cáo với nhóm để cùng xử lý.
4. Hạ tầng phục vụ phát triển và triển khai (máy chủ, domain, tài khoản dịch vụ, công cụ phát triển, license phần mềm...) phải là **tài sản riêng của cá nhân hoặc của nhóm**, có nguồn gốc rõ ràng.

## Điều 4. Quy hoạch Hệ sinh thái và nền tảng dùng chung

1. Hệ sinh thái được phát triển theo **quy hoạch thống nhất**, tránh tình trạng phát triển rời rạc, trùng lặp, không kế thừa được lẫn nhau.
2. Nhóm xây dựng và duy trì các **nền tảng dùng chung** phục vụ các nhóm tính năng chung. Hiện tại gồm:
   - **Sopbase** — nền tảng hạ tầng dùng chung: xác thực SSO (OAuth 2.0/OIDC), quản lý người dùng, phân quyền RBAC, danh mục dùng chung, lưu trữ file, audit log.
   - Các nền tảng dùng chung khác sẽ được bổ sung theo quy hoạch, dự kiến gồm: **nền tảng biểu mẫu động**, **nền tảng quy trình động (workflow)**, và các nền tảng khác do nhóm quyết định.
3. Nghĩa vụ của Sản phẩm thành phần đối với nền tảng dùng chung:
   - **Bắt buộc tích hợp và tái sử dụng** các tính năng mà nền tảng dùng chung đã cung cấp (ví dụ: đăng nhập SSO qua Sopbase, phân quyền RBAC, danh mục dùng chung, lưu trữ file); **không tự xây dựng lại** các tính năng này trừ khi có lý do kỹ thuật chính đáng được nhóm phê duyệt;
   - Khi một nền tảng dùng chung mới được ban hành, sản phẩm phát triển mới phải sử dụng ngay; sản phẩm hiện có phải lập **lộ trình chuyển đổi** và được nhóm thông qua;
   - Tuân thủ các quy ước kỹ thuật, tài liệu tích hợp do nhóm nền tảng ban hành.
4. Nhu cầu tính năng mang tính dùng chung (nhiều sản phẩm cùng cần) phải được đề xuất đưa vào nền tảng dùng chung thay vì phát triển riêng lẻ trong từng sản phẩm.
5. Nền tảng dùng chung là **tài sản chung của nhóm**; việc phát triển, vận hành và chi phí liên quan do nhóm thống nhất phân công và chia sẻ.

## Điều 5. Phê duyệt trước khi phát triển

1. Trước khi bắt đầu phát triển một Sản phẩm thành phần mới (hoặc một phân hệ lớn), thành viên phụ trách phải trình nhóm phê duyệt tối thiểu các nội dung:
   - **Danh mục tính năng** (phạm vi sản phẩm, các user stories/nhóm chức năng chính);
   - **Kiến trúc hệ thống** (công nghệ sử dụng, mô hình triển khai, phương án tích hợp với các nền tảng dùng chung);
   - Đối tượng khách hàng và sự phù hợp với quy hoạch Hệ sinh thái (không trùng lặp, chồng lấn với sản phẩm của thành viên khác).
2. Chỉ được bắt đầu phát triển **sau khi được phê duyệt**. Thay đổi lớn về phạm vi hoặc kiến trúc trong quá trình phát triển phải trình phê duyệt lại.

## Điều 6. Gia nhập Hệ sinh thái đối với sản phẩm có sẵn

1. Sản phẩm đã phát triển từ trước, muốn gia nhập Hệ sinh thái, phải thực hiện thủ tục: **đăng ký → đánh giá → phê duyệt**.
2. Hồ sơ đăng ký tối thiểu gồm: mô tả sản phẩm, danh mục tính năng, kiến trúc hệ thống, công nghệ sử dụng, hiện trạng khách hàng đang triển khai, hiện trạng bản quyền/sở hữu source code.
3. Tiêu chí đánh giá:
   - Phù hợp với quy hoạch Hệ sinh thái, không chồng lấn với sản phẩm hiện có (nếu chồng lấn, nhóm quyết định phương án hợp nhất hoặc phân định phạm vi);
   - Khả năng và lộ trình tích hợp các nền tảng dùng chung (tối thiểu là SSO qua Sopbase);
   - Chất lượng kỹ thuật, bảo mật, khả năng bảo trì;
   - Sở hữu trí tuệ rõ ràng, không có tranh chấp, không vi phạm Điều 3.
4. Sản phẩm được phê duyệt gia nhập phải cam kết lộ trình tích hợp nền tảng dùng chung với mốc thời gian cụ thể và chịu sự điều chỉnh của toàn bộ Thỏa thuận này như một Sản phẩm thành phần.

## Điều 7. Quản lý source code và tài liệu

1. Source code của mỗi Sản phẩm thành phần do thành viên phụ trách **tự quản lý riêng** trong quá trình phát triển.
2. Để đảm bảo Hệ sinh thái có thể duy trì lâu dài, mỗi Sản phẩm thành phần đã triển khai thực tế cho khách hàng phải có tối thiểu bộ tài liệu:
   - Tài liệu mô tả sản phẩm và danh mục tính năng;
   - Tài liệu kiến trúc hệ thống và công nghệ sử dụng (tech stack);
   - Tài liệu triển khai/cài đặt (deployment guide);
   - Tài liệu tích hợp với các nền tảng dùng chung.
3. Source code phải sử dụng hệ quản lý phiên bản (Git); khuyến khích **ký quỹ định kỳ** (backup/escrow) bản sao source code và tài liệu vào kho lưu trữ chung của nhóm để phòng rủi ro bất khả kháng (tai nạn, mất dữ liệu, thành viên đột ngột không thể tiếp tục).
4. Việc sử dụng thư viện/mã nguồn mở phải tuân thủ giấy phép tương ứng; không sử dụng thành phần có giấy phép gây rủi ro pháp lý cho việc thương mại hóa (nhóm sẽ liệt kê các loại giấy phép cần tránh khi cần).

## Điều 8. Cam kết hỗ trợ khách hàng và bàn giao khi ngừng tham gia

1. Sau khi Sản phẩm thành phần đã **triển khai thực tế cho khách hàng**, thành viên phụ trách phải lựa chọn và thực hiện một trong hai cam kết:
   - **(a) Hỗ trợ lâu dài:** tiếp tục bảo trì, sửa lỗi, hỗ trợ khách hàng và duy trì tương thích với các nền tảng dùng chung trong suốt vòng đời sản phẩm; hoặc
   - **(b) Bàn giao source code:** khi không tiếp tục tham gia, phải bàn giao lại toàn bộ source code, tài liệu, dữ liệu cấu hình, tài khoản hạ tầng liên quan để nhóm có thể duy trì và triển khai tiếp phần mềm.
2. Khi bàn giao theo điểm (b), thành viên được **thanh toán chi phí phát triển phần mềm tương ứng**. Phương án xác định chi phí do hai bên thỏa thuận tại thời điểm bàn giao, dựa trên các căn cứ tham khảo: khối lượng chức năng, công sức phát triển thực tế, doanh thu sản phẩm đang tạo ra, và mặt bằng chi phí phát triển phần mềm tương đương. Nếu không thống nhất được, xử lý theo Điều 13.
3. Điều kiện bàn giao được coi là hoàn tất khi:
   - Source code build/chạy được từ bản bàn giao, kèm hướng dẫn triển khai;
   - Đầy đủ tài liệu theo Điều 7 khoản 2;
   - Có tối thiểu **[30] ngày** hỗ trợ chuyển giao kỹ thuật cho người tiếp nhận.
4. Thành viên ngừng tham gia phải thông báo trước tối thiểu **[60] ngày**, và trong thời gian đó vẫn phải duy trì hỗ trợ khách hàng hiện có ở mức tối thiểu (sửa lỗi nghiêm trọng, đảm bảo hệ thống hoạt động).
5. Sau khi đã bàn giao và nhận thanh toán, thành viên không được sử dụng sản phẩm đã bàn giao để cạnh tranh trực tiếp với Hệ sinh thái, trừ khi được nhóm đồng ý bằng văn bản.

## Điều 9. Sở hữu trí tuệ và thương hiệu

1. Source code và tài sản trí tuệ của mỗi Sản phẩm thành phần thuộc về thành viên phụ trách phát triển, cho đến khi được bàn giao theo Điều 8 (khi đó chuyển giao cho nhóm hoặc bên tiếp nhận theo thỏa thuận).
2. Thương hiệu chung, domain, bộ nhận diện của Hệ sinh thái là **tài sản chung**, không thành viên nào được tự ý đăng ký sở hữu riêng, chuyển nhượng hoặc sử dụng ngoài phạm vi Hệ sinh thái.
3. Việc sử dụng thương hiệu chung để chào bán sản phẩm phải tuân theo quy tắc do nhóm thống nhất.

## Điều 10. Tài chính

1. Doanh thu từ mỗi Sản phẩm thành phần do thành viên phụ trách hưởng, **sau khi trích nộp phần đóng góp chung** theo tỷ lệ/mức do nhóm thống nhất (chi cho: vận hành nền tảng dùng chung, hạ tầng chung, marketing chung, quỹ dự phòng) *(tỷ lệ cụ thể quy định tại Phụ lục B)*.
2. Hợp đồng bán hàng có sự tham gia của nhiều Sản phẩm thành phần thì phân chia doanh thu theo thỏa thuận trước khi ký hợp đồng, ưu tiên theo tỷ trọng giá trị từng sản phẩm.
3. Mọi khoản thu chi chung phải được ghi chép và công khai định kỳ với toàn bộ thành viên.

## Điều 11. Chất lượng, bảo mật và dữ liệu khách hàng

1. Sản phẩm thành phần phải đáp ứng các yêu cầu tối thiểu trước khi triển khai cho khách hàng:
   - Kiểm soát truy cập, phân quyền đầy đủ (RBAC) ở cả frontend và backend;
   - Không lưu mật khẩu, khóa bí mật dạng rõ trong source code;
   - Có phương án sao lưu và khôi phục dữ liệu;
   - Ghi audit log cho các thao tác quan trọng (khuyến khích dùng dịch vụ audit log dùng chung của Sopbase).
2. Dữ liệu khách hàng thuộc về khách hàng; thành viên không được sử dụng dữ liệu khách hàng ngoài phạm vi hợp đồng với khách hàng đó, và phải tuân thủ pháp luật về bảo vệ dữ liệu cá nhân.

## Điều 12. Cơ chế quản trị và ra quyết định

1. Nhóm họp định kỳ **[hàng tháng]** để rà soát tiến độ, phê duyệt đề xuất và giải quyết vấn đề chung.
2. Các quyết định thông thường (phê duyệt sản phẩm mới, gia nhập hệ sinh thái, quy ước kỹ thuật) được thông qua khi có **quá bán** thành viên đồng ý.
3. Các quyết định hệ trọng (sửa đổi Thỏa thuận này, thay đổi tỷ lệ tài chính, kết nạp/chấm dứt thành viên, chuyển nhượng tài sản chung) cần tối thiểu **[2/3]** thành viên đồng ý.
4. Nhóm có thể bầu một **điều phối viên** nhiệm kỳ **[6–12 tháng]** để chủ trì họp, theo dõi cam kết và làm đầu mối quản lý tài sản chung.

## Điều 13. Xử lý vi phạm và giải quyết tranh chấp

1. Thành viên vi phạm Thỏa thuận (đặc biệt Điều 3 và Điều 8) sẽ bị nhắc nhở; vi phạm nghiêm trọng hoặc tái phạm có thể bị chấm dứt tư cách thành viên theo Điều 12 khoản 3, đồng thời vẫn phải thực hiện nghĩa vụ bàn giao theo Điều 8.
2. Tranh chấp giữa các thành viên ưu tiên giải quyết bằng **thương lượng nội bộ**; nếu không thành, nhóm họp toàn thể để biểu quyết phương án; trường hợp vẫn không giải quyết được thì thực hiện theo quy định pháp luật.
3. Thành viên vi phạm Điều 3 gây thiệt hại cho VNPT hoặc bên thứ ba tự chịu trách nhiệm cá nhân, nhóm và các thành viên khác không liên đới.

## Điều 14. Hiệu lực và sửa đổi

1. Thỏa thuận có hiệu lực kể từ ngày được toàn bộ thành viên sáng lập ký/xác nhận đồng ý.
2. Thành viên mới gia nhập phải xác nhận đồng ý với toàn bộ Thỏa thuận này.
3. Việc sửa đổi, bổ sung Thỏa thuận thực hiện theo Điều 12 khoản 3 và phải lập thành văn bản (phiên bản mới của tài liệu này, có ghi lịch sử thay đổi).

---

## Phụ lục A — Danh sách thành viên

| STT | Họ tên | Sản phẩm/nền tảng phụ trách | Ngày tham gia | Xác nhận |
|-----|--------|------------------------------|---------------|----------|
| 1 | *[...]* | *[...]* | *[...]* | |
| 2 | *[...]* | *[...]* | *[...]* | |

## Phụ lục B — Tỷ lệ đóng góp tài chính chung

*(Nhóm thống nhất và điền sau — ví dụ: trích X% doanh thu mỗi hợp đồng cho quỹ chung, hoặc mức đóng góp cố định/tháng cho vận hành nền tảng dùng chung.)*

## Lịch sử thay đổi

| Phiên bản | Ngày | Nội dung |
|-----------|------|----------|
| 1.0 | 12/07/2026 | Dự thảo lần đầu |
