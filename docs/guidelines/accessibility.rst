Khả năng tiếp cận
=================

TTO Design System cung cấp những đoạn code về khả năng tiếp cận (accessible) làm nền tảng cho TTO và các sản phẩm thuộc TTO.
Nhằm đảm bảo mọi thành phần đều có khả năng tiếp cận cao, bạn cần bám sát các hướng dẫn này, bao gồm hành vi sử dụng bàn phím cũng như quản lý các thuộc tính và vai trò ARIA của từng thành phần.

Khả năng tiếp cận là gì?
------------------------

Khả năng tiếp cận trong website đảm bảo người khuyết tật có thể nhận thức được, hiểu được, di chuyển được, tương tác được và sử dụng được ứng dụng web của bạn.
`Perceivable, Operable, Understandable and Robust <https://www.w3.org/TR/WCAG20/>`__.
Để đáp ứng điều này, một trang web cần cung cấp các thao tác bàn phím thay thế cho tất cả các thao tác bằng con trỏ chuột, nhận dạng rõ ràng tất cả các ô nhập dữ liệu và nút bấm, cung cấp từ ngữ thay thế cho tất cả các hình ảnh, video, biểu tượng, cũng như việc xây dựng các thành phần có khả năng tự diễn đạt cao.

TTO Design System cho phép phát triển các thành phần có khả năng tiếp cận cao bằng việc cung cấp các bộ thành phần chuẩn mực, mỗi thành phần đều đáp ứng tiêu chuẩn `ARIA <https://www.w3.org/TR/wai-aria/>`__, do đó chúng có thể được nhận diện chính xác bằng các công cụ hỗ trợ người khuyết tật.


Tuân thủ các bộ thành phần chuẩn
--------------------------------

Các thành phần trong TTO Design System và việc sử dụng các vai trò ARIA trong các thành phần đó dựa trên bộ tiêu chuẩn W3C và các tiêu chuẩn công nghiệp khác.


Điều hướng bàn phím
-------------------

Tất cả các tương tác bằng con trỏ chuột đều cần có thao tác bằng bàn phím tương ứng. Chúng tôi khuyến khích sử dụng các ngôn ngữ lập trình như Javascript để thực hiện điều này.


Sử dụng màu sắc hợp lý
----------------------

Tất cả các thành phần trong TTO Design System đều bám sát 2 nguyên tắc chính của màu sắc về khả năng tiếp cận:

* Không bao giờ chỉ sử dụng màu sắc để truyền đạt thông tin hay yêu cầu thao tác.
* Phối hợp giữa chữ và màu nền không thấp hơn ngưỡng khuyến nghị của `WCAG <https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-contrast.html>`__ với tỉ lệ 4.5:1 cho chữ thông thường và chữ nhỏ, và 3:1 cho chữ lớn.


Khả năng tiếp cận các ô nhập dữ liệu
------------------------------------

Tất cả các ô nhập dữ liệu đều sử dụng thẻ ``<fieldset>`` và ``<legend>`` và gắn nhãn hợp lý. Các ô lựa chọn và đánh dấu sử dụng một giải pháp cân bằng giữa khả năng tiếp cận và sự linh hoạt trong thiết kế.


Hình ảnh và biểu tượng
----------------------

Các hình ảnh và biểu tượng phải được cung cấp các câu chữ thay thế.


Nhận dạng thành phần
--------------------

Các thành phần tương tác được tạo ra dựa trên `ARIA Authoring Practices <http://w3c.github.io/aria/practices/aria-practices.html>`__ bao gồm các thuộc tính nhằm giúp những người sử dụng màn hình đọc chữ có thể hiểu được.


Xác thực khả năng tiếp cận
--------------------------

Sử dụng các công cụ xác thực khả năng tiếp cận hợp lý trước khi phát hành sản phẩm. Khuyến nghị dùng `WCAG Standard at the AA Level <https://www.w3.org/TR/WCAG20/#conformance>`__


Tài nguyên tham khảo
--------------------

* `W3C Web Accessibility Initiative <https://www.w3.org/WAI/>`__
* `WAI-ARIA Authoring Practices <http://w3c.github.io/aria/practices/aria-practices.html>`__
* `7 Things Every Designer Needs to Know about Accessibility <https://medium.com/salesforce-ux/7-things-every-designer-needs-to-know-about-accessibility-64f105f0881b#.o8n02j9rr>`__
* `Accessible Interface Design: on designing with accessible color contrast ratios <https://medium.com/salesforce-ux/accessible-interface-design-d80e95cbb2c1#.i5tl6ffv3>`__
* `WebAIM <http://webaim.org/>`__
* `The A11Y Project <http://a11yproject.com/>`__
