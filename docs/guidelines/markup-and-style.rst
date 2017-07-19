Markup và Style
===============

Các thành phần của TTO Design System được phát triển để lập trình viên có thể tạo ra giao diện đồng nhất trong tất cả các sản phẩm thuộc TTO bằng cách áp dụng những quy tắc CSS tiêu chuẩn.

Để đạt được điều đó, TTO Design System sử dụng kỹ thuật đặt tên đặc tả. Điều này giúp duy trì các đoạn code ngắn gọn, tính cụ thể thấp. TTO Design System dử dụng phương pháp đặt tên BEM, đi kèm một số quy ước bên dưới.

BEM Naming
----------

`BEM <https://en.bem.info/>`__ là một phương pháp đặt tên phổ biến: block, element, modifier.

Block
~~~~~

Một block đại diện cho tên một thành phần chính. Nếu bạn đang xây một ngôi nhà, tên class sẽ là ``.house``. Tất cả các thành phần thuộc ngôi nhà, sẽ được đặt tên dựa trên ``.house``.

Element
~~~~~~~

Một element đại diện cho một thành phần con, được ngăn cách với thành phần chính bằng 2 dấu gạch dưới. Cánh cửa trong ngôi nhà sẽ được đặt tên class là ``.house__door``. Cửa sổ sẽ là ``.house__window``.

Cẩn thận với các thành phần nhỏ hơn trong một thành phần lớn. Đặc biệt trong trường hợp có thể bị lặp lại bởi các thành phần không đồng cấp hoặc không liên quan. Tránh việc đặt tên như ``.house__stair__step``. Thay vào đó, hãy sử dụng ``.house__stair-step`` (dấu gạch nối dơn không biểu thị bất kỳ thành phần nào trong BEM, và có thể sử dụng để đặt tên nhóm các thành phần). Hoặc nếu các thành phần của cầu thang (stair) có thể được sử dụng trong một thành phần khác, lúc đó sử dụng ``.stair`` như một thành phần lớn, và tạo các thành phần nhỏ hơn ``.stair__step``.


Modifier
~~~~~~~~

Một modifier là một biến thể của thành phần hoặc phần tử, và được ngăn cách bằng một dấu gạch dưới. Biến thể có thể được sử dụng cho các thành phần tổng quan, hoặc có thể áp dụng cho một phần tử bên trong thành phần khác.

Vì các thuộc tính nên được áp dụng cho tất cả các ngôi nhà ``.house``, do vậy các ngôi nhà đều có tên class ``.house``. Nếu một ngôi nhà nào đó có một đặc điểm khác, ví dụ nhà màu xám, ``.house_grey`` sẽ được thêm vào bên cạnh tên class ``.house`` đang có. ``.house .house_grey``.

Nếu ngôi nhà có cửa màu hồng, biến thể có thể được đặt ngay tại tên của phần tử đó, ``.house__door__pink``.

