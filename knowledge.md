- Cùng cấp _./_
- Truy xuất ra ngoài 1 cấp _../_
- Thuộc tính _attribute_
- CSS nó sẽ chạy từ trên xuống dưới, nếu có 2 đoạn code cùng thực hiên 1 chức năng thì nó sẽ ưu tiên đoạn code ở dưới
- _div_ là thẻ block, có độ rộng 100% phần tử chứa nó, lưu ý: chưa nói tới vấn đề khi sử dụng với CSS
- _div_ thường được dùng rất nhiều, khi chia layout, gom 1 khối nào đó
- _img_ là thẻ inline, tự đóng, dùng để hiển thị hình ảnh với 2 thuộc tính là `src` và `alt`
- _alt_ viết tắt của `alternate text` nó dùng trong việc SEO, khi hình ảnh bị lỗi hoặc sai đường dẫn thì _alt_ sẽ hiển thị để người dùng biết hình ảnh đó nói về cái gì
- _span_ là thẻ inline, nó thường được dùng cho những đoạn chữ ngắn
- _class_ là thuộc tính dùng để sử dụng các class cho thẻ, sau đó dùng để styles trong CSS
- Việc đặt tên class khá là nan giải, khó, ko nên đặt tên tiếng Việt, nên đặt tiếng Anh ngắn gọn dễ hiểu
- Thẻ tiêu đề: h1, h2, h3, h4, h5, h6
- _h1_: Mỗi trang chỉ có tối đa 1 thẻ h1 mà thôi, thẻ này thường được dùng cho những tiêu đề lớn của trang
- _h2_: Dùng được nhiều, thường được dùng cho những block to
- _h3_: Dùng được nhiều, thường được dùng cho những block nhỏ
- h4,h5,h6: Tương ứng cho những tiêu đề nhỏ hơn
- _a_: Là thẻ inline, chắc chắn là dùng cho liên kết, nó có 3 thuộc tính hay dùng `href`, `target`, và `rel`
- Khi dùng `target` có giá trị là `_blank` thì thẻ a nên thêm thuộc tính `rel="noopener noreferrer"`
- Fonts chữ:
- 1. Sẽ có sẵn ở Google Fonts
- 2. Không có ở Google Fonts mà được mua, tải trên mạng về máy
- _font-weight_: Độ đậm nhạt của chữ, 100 -> 900, normal, bold, bolder, extra bold, light, thin, regular, medium, semibold
- _font-family_: Thiết lập font chữ, truyền vào là font name(tên của font chữ)
- `sans-serif`: Chữ không có chân
- `serif`: Chữ có chân
- _CSS Selectors_: tag, class, id, attribute
- Tags: h1, h2, h3, div, body, span, a
- Class: .name, .tour, .tour-header
- Id: #header, #content
- Attribute: Later `*`
- Special selector: \* chọn toàn bộ selectors
- Cấu trúc 1 đoạn code CSS
  cssSelectors, cssSelectors, cssSelectors{
  property: value;
  }
  h1,.name,#header,input[type='email']{
  font-family: 'Inter'
  }
- _User Agent Stylesheet_: CSS mặc định của trình duyệt, mỗi trình duyệt sẽ có CSS mặc định khác nhau
- _CSS reset_: Dùng để reset CSS mặc định của các trình duyệt
- _box-sizing_: margin, padding, border, width, height, đơn vị px
- _color_:
- _background-color_:
-
