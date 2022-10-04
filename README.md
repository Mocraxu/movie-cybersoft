# Movie Project:

Dự án được thực hiện bằng reactJS trong suốt quá trình học tại trung tâm CyberSoft, APIs được cung cấp từ CyberSoft. Dự án gồm một số trang và chức năng chính như: 
  - Trang chủ, trang đặt vé 
  - Trang đăng ký/đăng nhập người dùng 
  - Trang Admin: - Thêm xoá sửa phim 
  - Thêm xoá sửa người dùng

## Structure

- public
  - assets/img: chứa file hình ảnh dùng cho trang web
- src
  - components: Chứa các common component dùng chung cho toàn bộ trang web.
  - data: Chứa dữ liệu mảng của các đối tượng dùng trong trang web.
  - pages: Chứa các trang web hoặc chức năng như: trang chủ, trang admin, trang đặt vé, trang đăng nhập/đăng ký, xác minh thông tin tài khoản.
  - redux:
    - actions: Chứa redux actions
    - constants: Chứa redux action types/ Chứa những biến constants sử dụng trong module
    - reducers: Chứa redux reducers
    - configStore.js: Setup redux store
  - routers: Cấu hình các địa chỉ dẫn đến trang web, Sử dụng kĩ thuật lazyload
  - services:
    - Cấu hình các phương thức gọi API (axios, fetch)
    - Chứa các tác vụ liên quan đến gọi API
  - template: Chứa các thành phần nhỏ dùng chung cho toàn bộ trang web: header, footer, navbar ...
  - utils: Chứa các common function của js dùng chung cho ứng dụng
  - App.js:
    - Gom các component dùng cho toàn bộ trang web.
    - Global component: ErrorBoudary, Auth...
  - index.js: cung cấp store cho toàn bộ trang web
  - index.css: Setup global styles

### Library
- Store: react-redux
- Router: react-router-dom
- UI component: MUI
- Style:
  - CSS
  - CSS-in-JS: styled-component/@emotion
- Validation:
  - Schema
  - Yup
- Other:
  - axios: xử lý APIs
  - lodash: thư viện giúp thao tác với các mảng thuận tiện hơn
  - moment: xử lý định dạng thời gian
  ...