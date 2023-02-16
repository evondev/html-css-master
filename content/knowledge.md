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
- _CSS reset_: Dùng để reset CSS mặc định của các trình duyệt, và 'bắt buộc' phải có đầu tiên
- _color_: Màu chữ
- _background-color_: Màu nền
- _Mã màu_: hexa(#ffa400), orange, rgb(0,0,0), rgba(0,0,0,0.5)
- _Alpha_(opacity): 0 -> 1
- **box-sizing**
- _content-box_: Độ rộng lúc này của 1 khối sẽ bằng width + padding(left+right) + border(left+right)
- _border-box_: Độ rộng lúc này của 1 khối sẽ bao gồm padding và border, nên áp dụng cho toàn bộ selector(\*)
- _width_: Độ rộng
- _height_: Chiều cao
- _border_: Viền
- _shorthand_: (CSS shorthand) Viết rút gọn
- _padding_: Không thể dùng số âm
- _margin_: Có thể dùng số âm, có giá trị `auto`
- _text-decoration_: Gạch dưới của thẻ a, `none`, `underline`, `overline`,` line-through`
- _border-radius_: Độ bo góc của khối, càng lớn thì càng bo góc, nếu hình vuông mà có bo góc lớn thì sẽ tạo ra hình tròn, còn nếu là hình chữ nhật có bo góc lớn thì sẽ tạo ra hình elip
- border-top-left-radius, border-top-right-radius, border-bottom-left-radius, border-bottom-right-radius
- _line-height_: Khoảng cách giữa các dòng chữ
- Khi những thẻ inline nằm cạnh nhau thì nó sẽ nằm trên 1 hàng, ngược lại những thẻ block thì nó sẽ tạo ra hàng mới
- _display_: block, inline, inline-block, none, flex, grid
- `block` : Biến thành thẻ block
- `inline` : Biến thành thẻ inline, nó sẽ bị hạn chế vài thuộc tính CSS liên quan tới box-sizing như là padding-top, padding-bottom, margin-top, margin-bottom
- `inline-block` : Biến thành thẻ inline-block,
  là sự kết hợp giữa inline và block, khi các thẻ có thuộc tính inline-block nó sẽ kế thừa đặc tính của inline tức là nằm cạnh nhau thì sẽ nằm trên 1 hàng, có độ rộng bằng nội dung mà nó chứa, không bị hạn chế CSS
- `none`: Ẩn luôn, ko thấy ko nhấn được
- `flex`: Dùng rất nhiều hiện nay, nếu master được nó thì code layout vô tư :D
- _min-width_: Độ rộng tối thiểu, ví dụ 100px -> >= 100px
- _max-width_: Độ rộng tối đa, ví dụ 100px -> <= 100px
- _flexbox_: Áp dụng thuộc tính display: flex vào phần tử mình muốn dàn layout
- _calc_: Hàm dùng để tính toán, + - \* /, lưu ý là phải có khoảng cách giữa các phép tính
- _column-gap_: Khoảng trống chiều dọc
- _row-gap_: Khoảng trống chiều ngang
- _component_: Mục đích là tái sử dụng và có thể tùy chỉnh 1 chỗ để sử dụng nhiều nơi
- _pug_: https://pugjs.org/api/getting-started.html
- mixins: Giống function trong Javascript mục đích là tái sử dụng code
- Biến: =, #{biến}
- _position_: có 5 giá trị chính: static, relative, absolute, sticky, fixed, khi sử dụng thuộc tính position này thì đi kèm sẽ có các thuộc tính khác như top right bottom left z-index
- _relative_: Khi sử dụng giá trị này thì phải lưu ý xem phần tử con của nó có sử dụng position là `absolute` hay không ?
- _absolute_: Khi sử dụng giá trị này thì phải lưu ý xem phần tử chứa nó gần nhất có sử dụng position là absolute hay relative không ?
- _responsive_:
- _breakpoints_: 320px 480px 768px 1024px 1200 1366 1440 1600 1920
- _min-width_: breakpoints
- _max-width_: breakpoints - 0.02px
- _media queries_
- _variables_: Biến là gì ? Khai báo như thế nào ? Cách sử dụng ra sao ? Ưu và nhược điểm của nó là gì ?
- _grid_: Dàn layout cực nhanh
- _time_: nó là thẻ inline
- _each in pug_: Dùng để duyệt qua danh sách các phần tử trong mảng để hiển thị
- _object-fit_: Thuộc tính này dùng cho thẻ img hoặc video, mục đích là để hiển thị hình ảnh hoặc video vừa với khung chứa nó hay không?
- _object-position_: Dùng để căn chỉnh vị trí hiển thị của img hoặc video khi dùng với thuộc tính `object-fit`
- _css selectors child_: :nth-child(number), :nth-last-child(number), :first-child, :last-child, những phần tử cùng cấp, .gem-item:first-child, .gem-item:last-child, .gem-item:nth-child(5), :not(selectors), .gem-item:not(:first-child), .gem-item:not(:nth-child(5))
  pug index.pug --pretty --watch
- _width: fit-content_: có độ rộng bằng với nội dung nó chứa
- _margin-inline_: tương ứng margin-left và margin-right
- _padding-inline_: tương ứng padding-left và padding-right
- _margin-block_: tương ứng margin-left và margin-right
- _padding-block_: tương ứng padding-top và padding-bottom
- _caniuse_: là 1 trang web giúp chúng ta kiểm tra những thuộc tính trong css xem nó có được nhiều trình duyệt hỗ trợ hay không ? Từ đó chúng ta có thể chắc chắn sử dụng vào trong dự án
- _semantic tags_: header, footer, main, section, article, nav, aside
- _list-style-type_: thuộc tính này dùng cho thẻ ul(`disc`) và ol(`decimal`)
- _list-style-position_: outside hoặc inside
- _form_: dùng để làm các form(biểu mẫu) nhập thông tin để làm việc gì đó ví dụ như đăng ký tài khoản, đăng nhập, gửi email, điền thông tin cá nhân...
- _input_: có thuộc tính(attribute), và nó là thẻ tự đóng
- `type` có nhiều loại tùy thuộc vào mục đích chúng ta sử dụng: text, email, number, phone, time, date, file, password, checkbox, radio, submit...
- `placeholder` 1 lớp chữ giả mờ để nói cho chúng ta biết input đó làm gì, `name` dùng để truy xuất dữ liệu
- `required` bắt buộc,
- `disabled` không cho phép nhập vào, và khi submit form nó cũng ko lấy được dữ liệu,
- `readonly` chỉ đọc, không sửa được tuy nhiên khi submit form thì vẫn lấy được dữ liệu
- `min` thường dùng cho number, tức là số nhỏ nhất
- `max` tương tự ở dòng trên nhưng là số lớn nhất
- `min-length` tối thiểu kí tự
- `max-length` tối đa kí tự
- button
- `type`: button, submit, reset
- `inputmode`: _search_ _tel_ _number_ _decimal_ _email_ _url_
- `autocomplete`: tự động điền, _on_ _off_
- Trạng thái của input có `focus` `valid` `invalid` `out-of-range`...
- Button có `hover`, `focus` `active` `disabled`
- _select_: thường sẽ được tùy biến lại bằng cách dùng ul li
- _textarea_: thường dùng cho nội dung nhập nhiều và có xuống hàng, thư viện soạn thảo hay gặp là `ckeditor`
- _transition_: làm cho chuyển động trở nên mượt mà hơn, transition: property(all, color, background-color) duration(100ms, 200ms, 2s, 3s) easing(linear, ease, ease-in, ease-in-out, ease-out, cubic bezier)
- _flex-shrink_: nếu để giá trị là `0` thì độ rộng hoặc chiều cao của nó cố định tại kích thước mình thiết lập và không bị bóp lại
- _flex-grow_: nếu giá trị là `1` thì cho phép giãn ra
- _flex-basis_: nó sẽ là độ rộng(flex-direction: row) hoặc là chiều cao(flex-direction: column)
- _minmax_
- _auto-fit_ vs _auto-fill_
- pseudo: `:hover`

# Những thứ khó nắm vững

- clamp min max
- Responsive
- Container queries
- Conditional CSS

# Commands

- sass ./sass/main.scss ./css/main.css --watch
- pug index.pug --pretty --watch
