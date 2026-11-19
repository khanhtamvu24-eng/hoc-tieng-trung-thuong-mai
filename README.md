# Học tiếng Trung Thương mại 🌸

Bộ công cụ tự học tiếng Trung cho dân Thu mua (Procurement), dựa trên giáo trình *基础实用商务汉语 (第三版) 上册* (Giáo trình tiếng Trung Thương mại, bản thứ 3, tập 1).

## Có gì trong repo

| Thư mục | Nội dung |
|---|---|
| `docs/index.html` | Web học từ vựng mỗi ngày, tông hồng. Gồm 42 từ và 6 danh từ riêng của Bài 1 (到达中国 · Đến Trung Quốc), có ví dụ thu mua viết thành 3 dòng Hán – Pinyin – Việt. |
| `skills/chinese-procurement-coach/SKILL.md` | Skill "Coach tiếng Trung Thu mua" cho Claude: luyện từ vựng, đóng vai Supplier / Chủ đầu tư, sửa tin nhắn WeChat. |

## Web học từ vựng

Tính năng:

- **Học hôm nay:** mỗi ngày vài từ mới cộng với các từ đến hạn ôn.
- **Ôn ngắt quãng:** từ đã nhớ quay lại sau 1 → 2 → 4 → 7 → 15 → 30 ngày.
- **5 dạng luyện tập:** nhìn chữ đoán nghĩa, nghĩa → chữ Hán, chữ Hán → pinyin, nghe chọn chữ, điền từ vào câu.
- **Lộ trình:** chuỗi ngày học 🔥, mục tiêu XP và dự báo 7 ngày tới.
- **Sổ từ:** tìm được cả khi gõ không dấu, nghe phát âm từng từ.
- **Nhật ký học:** lưu lại từ đã học theo từng ngày, xem lại và ôn lại riêng từng ngày.

### Mở web bằng GitHub Pages

1. Vào **Settings → Pages** của repo.
2. Ở **Source**, chọn **Deploy from a branch**, branch `main`, thư mục `/docs`, rồi bấm **Save**.
3. Sau khoảng 1 phút, web chạy tại `https://<tên-tài-khoản>.github.io/<tên-repo>/`.

Khi chạy ngoài claude.ai, tiến độ được lưu trong trình duyệt (localStorage) và phát âm dùng giọng tiếng Trung có sẵn của trình duyệt. Mỗi thiết bị giữ tiến độ riêng.

Bạn cũng có thể tải `docs/index.html` về máy và mở trực tiếp bằng trình duyệt.

## Dùng skill với Claude

Tải thư mục `skills/chinese-procurement-coach` lên phần Skills trong cài đặt Claude, hoặc chép vào `~/.claude/skills/` nếu dùng Claude Code.

Các từ khóa kích hoạt chế độ: `[Trình mẫu]`, `[Đàm phán Supplier]`, `[Từ vựng chuyên ngành]`, `[Sửa tin nhắn/Email]`, `[Giao tiếp hằng ngày]`.

## Thêm bài mới

Từ vựng nằm trong mảng `W` ở đầu phần `<script>` của `docs/index.html`. Mỗi từ là một dòng:

```js
["id","汉字","pīnyīn","nghĩa","câu ví dụ","pinyin câu","nghĩa câu","từ trong câu","g1","thành phần con (tuỳ chọn)"]
```
