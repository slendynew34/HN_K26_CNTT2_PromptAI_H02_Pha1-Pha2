# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 04
- **Họ tên:** Pham Vu Tuan Kiet
- **Lớp:**CNTT2
- **Link repository Pha2:**https://github.com/slendynew34/HN_K26_CNTT2_PromptAI_H02_Pha1-Pha2/blob/main/bai_lam_pha2.md
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):**Gemini

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt vé xe ra JSON

**KET QUA AI**

```text
{
  "TN1": {
    "ma_tuyen": "SGDL",
    "ngay_di": "2026-12-22",
    "ve_nguoi_lon": 2,
    "ve_tre_em": 1,
    "loai_cho": "giuong",
    "ghi_chu": null
  },
  "TN2": {
    "ma_tuyen": "SGNT",
    "ngay_di": "2027-01-02",
    "ve_nguoi_lon": 3,
    "ve_tre_em": 0,
    "loai_cho": null,
    "ghi_chu": "một người đang mang thai 6 tháng"
  },
  "TN3": {
    "ma_tuyen": "SGCT",
    "ngay_di": null,
    "ve_nguoi_lon": 4,
    "ve_tre_em": 0,
    "loai_cho": "ghe",
    "ghi_chu": "bà nội đi xe lăn"
  }
}```

**Link trò chuyện:**https://share.gemini.google/mFCcmaeKHnod

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
- Bước 1: Xác định đơn giá gói vé và đơn giá vé theo nhóm tuổi.
  + Đơn giá gói vé SVT cho người lớn: 1.200.000 VNĐ/người.
  + Đơn giá trẻ em từ 5–11 tuổi (tính 70% giá vé người lớn): 1.200.000 × 70% = 840.000 VNĐ/trẻ.
  + Đơn giá trẻ em dưới 5 tuổi: Miễn phí (0 VNĐ/trẻ).

- Bước 2: Tính tiền vé người lớn và trẻ em, cộng tổng tiền trước giảm.
  + Tiền vé người lớn (5 người): 5 × 1.200.000 = 6.000.000 VNĐ.
  + Tiền vé trẻ em 5–11 tuổi (2 trẻ): 2 × 840.000 = 1.680.000 VNĐ.
  + Tiền vé trẻ em dưới 5 tuổi (1 trẻ): 1 × 0 = 0 VNĐ.
  => Tổng tiền vé trước giảm = 6.000.000 + 1.680.000 + 0 = 7.680.000 VNĐ.

- Bước 3: Kiểm tra điều kiện giảm giá nhóm, tính số tiền giảm và tiền sau giảm.
  + Điều kiện: Đoàn có 5 người lớn (đạt mốc từ 5 người lớn trở lên) nên được áp dụng mức giảm giá nhóm 5% trên tổng tiền vé.
  + Số tiền được giảm: 7.680.000 × 5% = 384.000 VNĐ.
  => Tiền vé sau giảm = 7.680.000 - 384.000 = 7.296.000 VNĐ.

- Bước 4: Tính tiền phụ thu khu ghế ưu tiên (nếu có).
  + Có 1 người lớn đăng ký ghế ưu tiên với mức phụ thu 300.000 VNĐ/người (khoản phụ thu này không áp dụng giảm giá nhóm).
  => Tiền phụ thu = 1 × 300.000 = 300.000 VNĐ.

- Bước 5: Cộng tiền vé sau giảm với phụ thu để ra TỔNG TIỀN cuối cùng.
  => TỔNG TIỀN = 7.296.000 + 300.000 = 7.596.000 VNĐ.
```

**Link trò chuyện:**https://share.gemini.google/UMJO4np8Tfnf

### b) Kiểm tra kết quả AI

Đánh giá tính chính xác: Kết quả AI tính toán chính xác hoàn toàn ở tất cả các bước so với quy tắc và bảng giá của ban tổ chức.

Chi tiết đối chiếu:

Phân loại đối tượng & đơn giá: AI áp dụng đúng mức giá gốc gói SVT (1.200.000 VNĐ), tính đúng tỷ lệ 70% cho trẻ 5–11 tuổi (840.000 VNĐ) và miễn phí cho trẻ dưới 5 tuổi.

Điều kiện ưu đãi nhóm: AI đếm đúng số lượng người lớn là 5 người (không gộp trẻ em vào để tính điều kiện) nên đủ điều kiện giảm 5%.

Tách biệt khoản phụ thu: AI không gộp phí phụ thu ghế ưu tiên (300.000 VNĐ) vào tổng tiền trước giảm mà cộng riêng ở Bước 4, tuân thủ đúng quy định không chiết khấu trên phụ thu, cho ra con số cuối cùng là 7.596.000 VNĐ.

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
(Dán câu trả lời của AI vào đây (bấm nút Copy dưới câu trả lời) – xoá dòng này)
```

**Link trò chuyện:**

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
(Dán câu trả lời của AI vào đây (bấm nút Copy dưới câu trả lời) – xoá dòng này)
```

**Link trò chuyện:**
