# 🏆 SPORT SHOP - WEBSITE BÁN ĐỒ THỂ THAO

Website thương mại điện tử chuyên bán các sản phẩm đồ thể thao như quần áo, giày, bóng, phụ kiện và dụng cụ tập luyện.

## 📌 Mục lục

* [Giới thiệu](#-giới-thiệu)
* [Chức năng](#-chức-năng)
* [Công nghệ sử dụng](#-công-nghệ-sử-dụng)
* [Cấu trúc dự án](#-cấu-trúc-dự-án)
* [Cài đặt](#-cài-đặt)
* [Cấu hình](#-cấu-hình)
* [Cơ sở dữ liệu](#-cơ-sở-dữ-liệu)
* [API](#-api)
* [Tài khoản mẫu](#-tài-khoản-mẫu)
* [Quy trình mua hàng](#-quy-trình-mua-hàng)
* [Phân quyền](#-phân-quyền)
* [Đóng góp](#-đóng-góp)
* [Tác giả](#-tác-giả)

---

## 📖 Giới thiệu

**Sport Shop** là website bán đồ thể thao được xây dựng nhằm cung cấp một nền tảng mua sắm trực tuyến tiện lợi cho khách hàng.

Website hỗ trợ khách hàng:

* Xem danh sách sản phẩm.
* Tìm kiếm sản phẩm.
* Lọc sản phẩm theo danh mục.
* Xem chi tiết sản phẩm.
* Thêm sản phẩm vào giỏ hàng.
* Đặt hàng.
* Theo dõi đơn hàng.
* Quản lý thông tin cá nhân.

Đối với quản trị viên, hệ thống hỗ trợ:

* Quản lý sản phẩm.
* Quản lý danh mục.
* Quản lý khách hàng.
* Quản lý đơn hàng.
* Quản lý tồn kho.
* Quản lý khuyến mãi.
* Theo dõi doanh thu.

---

## ✨ Chức năng

### 🛍️ Khách hàng

* Đăng ký tài khoản.
* Đăng nhập / đăng xuất.
* Quên mật khẩu.
* Xem sản phẩm.
* Tìm kiếm sản phẩm.
* Lọc theo danh mục.
* Sắp xếp theo giá.
* Xem chi tiết sản phẩm.
* Chọn size / màu sắc.
* Thêm vào giỏ hàng.
* Cập nhật số lượng.
* Xóa sản phẩm khỏi giỏ hàng.
* Đặt hàng.
* Xem lịch sử mua hàng.
* Theo dõi trạng thái đơn hàng.
* Đánh giá sản phẩm.

### 👟 Sản phẩm

Các nhóm sản phẩm:

* 👕 Áo thể thao
* 👖 Quần thể thao
* 👟 Giày thể thao
* ⚽ Bóng thể thao
* 🏀 Dụng cụ bóng rổ
* 🏸 Dụng cụ cầu lông
* 🏋️ Dụng cụ tập gym
* 🎒 Balo & túi thể thao
* 🧢 Phụ kiện thể thao

Thông tin sản phẩm gồm:

* Tên sản phẩm.
* Hình ảnh.
* Giá bán.
* Giá khuyến mãi.
* Mô tả.
* Danh mục.
* Thương hiệu.
* Size.
* Màu sắc.
* Số lượng tồn kho.
* Trạng thái sản phẩm.

---

## 🛒 Giỏ hàng

Khách hàng có thể:

* Thêm sản phẩm vào giỏ.
* Chọn số lượng.
* Thay đổi size.
* Thay đổi màu sắc.
* Xóa sản phẩm.
* Xem tổng tiền.
* Áp dụng mã giảm giá.

Ví dụ:

```text
┌─────────────────────────────────────┐
│              GIỎ HÀNG               │
├─────────────────────────────────────┤
│ 👟 Nike Air Max                     │
│    Size: 42 | SL: 1                 │
│    2.500.000 VNĐ                     │
├─────────────────────────────────────┤
│ 👕 Áo thể thao                       │
│    Size: L | SL: 2                   │
│      800.000 VNĐ                     │
├─────────────────────────────────────┤
│ Tổng tiền:          3.300.000 VNĐ   │
│                                     │
│          [ TIẾN HÀNH ĐẶT HÀNG ]     │
└─────────────────────────────────────┘
```

---

## 📦 Quản lý đơn hàng

Trạng thái đơn hàng:

```text
PENDING
   ↓
CONFIRMED
   ↓
PROCESSING
   ↓
SHIPPING
   ↓
DELIVERED
```

Ngoài ra:

```text
PENDING → CANCELLED
```

Khách hàng có thể xem:

* Mã đơn hàng.
* Ngày đặt.
* Danh sách sản phẩm.
* Số lượng.
* Tổng tiền.
* Địa chỉ giao hàng.
* Phương thức thanh toán.
* Trạng thái đơn hàng.

---

## 💳 Thanh toán

Hệ thống có thể hỗ trợ:

* Thanh toán khi nhận hàng (COD).
* Chuyển khoản ngân hàng.
* Thanh toán online.

> Các phương thức thanh toán online cần được cấu hình riêng theo cổng thanh toán được sử dụng.

---

## 🎁 Khuyến mãi

Admin có thể tạo:

* Mã giảm giá theo phần trăm.
* Mã giảm giá theo số tiền.
* Giảm giá theo sản phẩm.
* Giảm giá theo danh mục.
* Chương trình khuyến mãi theo thời gian.

Ví dụ:

```text
SPORT10

Giảm: 10%
Đơn tối thiểu: 500.000 VNĐ
Thời gian: 01/08/2026 - 31/08/2026
```

---

## 👨‍💼 Chức năng Admin

### Dashboard

Admin có thể xem:

* Tổng doanh thu.
* Tổng đơn hàng.
* Tổng sản phẩm.
* Tổng khách hàng.
* Đơn hàng mới.
* Sản phẩm bán chạy.
* Doanh thu theo ngày / tháng / năm.

### Quản lý sản phẩm

```text
GET    /api/products
GET    /api/products/:id
POST   /api/products
PUT    /api/products/:id
DELETE /api/products/:id
```

### Quản lý danh mục

```text
GET    /api/categories
POST   /api/categories
PUT    /api/categories/:id
DELETE /api/categories/:id
```

### Quản lý đơn hàng

```text
GET    /api/orders
GET    /api/orders/:id
PUT    /api/orders/:id
DELETE /api/orders/:id
```

---

## 🛠 Công nghệ sử dụng

### Frontend

* HTML5
* CSS3
* JavaScript
* ReactJS
* Bootstrap / Tailwind CSS

### Backend

* Node.js
* Express.js

### Database

* MySQL

### Authentication

* JWT
* bcrypt

### Công cụ

* Git
* GitHub
* VS Code
* Postman

---

## 📁 Cấu trúc dự án

```text
sport-shop/
│
├── frontend/
│   ├── public/
│   └── src/
│       ├── assets/
│       ├── components/
│       ├── pages/
│       ├── layouts/
│       ├── services/
│       ├── hooks/
│       ├── context/
│       ├── utils/
│       └── App.jsx
│
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── services/
│   ├── utils/
│   └── server.js
│
├── database/
│   ├── schema.sql
│   └── seed.sql
│
├── uploads/
│
├── .env.example
├── .gitignore
└── README.md
```

---

## 🚀 Cài đặt

### 1. Clone project

```bash
git clone https://github.com/username/sport-shop.git

cd sport-shop
```

### 2. Cài đặt Backend

```bash
cd backend
npm install
```

### 3. Cài đặt Frontend

```bash
cd ../frontend
npm install
```

### 4. Tạo Database

Tạo database MySQL:

```sql
CREATE DATABASE sport_shop;
```

Sau đó import:

```text
database/schema.sql
database/seed.sql
```

---

## ⚙️ Cấu hình

Tạo file `.env` trong thư mục `backend`:

```env
PORT=5000

DB_HOST=localhost
DB_PORT=3306
DB_NAME=sport_shop
DB_USER=root
DB_PASSWORD=your_password

JWT_SECRET=your_secret_key

CLIENT_URL=http://localhost:3000
```

---

## ▶️ Chạy project

### Backend

```bash
cd backend
npm run dev
```

Backend:

```text
http://localhost:5000
```

### Frontend

```bash
cd frontend
npm run dev
```

Frontend:

```text
http://localhost:3000
```

---

## 🗄️ Cơ sở dữ liệu

Các bảng chính:

| Bảng               | Mô tả                 |
| ------------------ | --------------------- |
| `users`            | Tài khoản             |
| `customers`        | Khách hàng            |
| `categories`       | Danh mục              |
| `brands`           | Thương hiệu           |
| `products`         | Sản phẩm              |
| `product_variants` | Size / màu / biến thể |
| `inventory`        | Tồn kho               |
| `carts`            | Giỏ hàng              |
| `cart_items`       | Chi tiết giỏ hàng     |
| `orders`           | Đơn hàng              |
| `order_items`      | Chi tiết đơn hàng     |
| `payments`         | Thanh toán            |
| `reviews`          | Đánh giá              |
| `coupons`          | Mã giảm giá           |

### Quan hệ cơ bản

```text
User
 │
 └── Customer
       │
       ├── Cart
       │    └── CartItem
       │         └── Product
       │
       └── Order
            ├── OrderItem
            │     └── Product
            │
            └── Payment

Category
   │
   └── Product
          │
          └── ProductVariant
                 └── Inventory
```

---

## 🔐 Phân quyền

| Vai trò    | Quyền                         |
| ---------- | ----------------------------- |
| `ADMIN`    | Quản lý toàn bộ hệ thống      |
| `STAFF`    | Quản lý sản phẩm và đơn hàng  |
| `CUSTOMER` | Mua hàng và quản lý tài khoản |

---

## 👤 Tài khoản mẫu

> Chỉ sử dụng trong môi trường development.

| Vai trò  | Email                  | Mật khẩu       |
| -------- | ---------------------- | -------------- |
| Admin    | `admin@example.com`    | `Admin@123`    |
| Staff    | `staff@example.com`    | `Staff@123`    |
| Customer | `customer@example.com` | `Customer@123` |

**Không sử dụng các tài khoản/mật khẩu mẫu này trong production.**

---

## 🔄 Quy trình mua hàng

```text
Khách hàng
    │
    ▼
Xem sản phẩm
    │
    ▼
Chọn sản phẩm
    │
    ▼
Chọn Size / Màu
    │
    ▼
Thêm vào giỏ hàng
    │
    ▼
Kiểm tra giỏ hàng
    │
    ▼
Nhập thông tin giao hàng
    │
    ▼
Chọn phương thức thanh toán
    │
    ▼
Xác nhận đơn hàng
    │
    ▼
      Đặt hàng
    │
    ▼
Admin xác nhận
    │
    ▼
Đóng gói
    │
    ▼
Giao hàng
    │
    ▼
Hoàn thành
```

---

## 📡 API chính

### Authentication

```http
POST /api/auth/register
POST /api/auth/login
POST /api/auth/logout
GET  /api/auth/me
```

### Products

```http
GET    /api/products
GET    /api/products/:id
POST   /api/products
PUT    /api/products/:id
DELETE /api/products/:id
```

### Categories

```http
GET    /api/categories
POST   /api/categories
PUT    /api/categories/:id
DELETE /api/categories/:id
```

### Cart

```http
GET    /api/cart
POST   /api/cart/items
PUT    /api/cart/items/:id
DELETE /api/cart/items/:id
```

### Orders

```http
GET  /api/orders
GET  /api/orders/:id
POST /api/orders
PUT  /api/orders/:id/status
```

### Reviews

```http
GET  /api/products/:id/reviews
POST /api/products/:id/reviews
```

---

## 🧪 Testing

Chạy unit test:

```bash
npm test
```

Kiểm tra API bằng:

```text
Postman
```

---

## 📦 Build Production

Frontend:

```bash
npm run build
```

Backend:

```bash
npm start
```

---

## 🔒 Bảo mật

* Mật khẩu được mã hóa bằng `bcrypt`.
* Authentication sử dụng JWT.
* Kiểm tra quyền truy cập API.
* Validate dữ liệu đầu vào.
* Không lưu mật khẩu dạng plaintext.
* Không commit file `.env`.
* Kiểm tra dữ liệu trước khi tạo đơn hàng.
* Kiểm tra tồn kho trước khi thanh toán.

---

## 📱 Các trang chính

```text
/
├── Trang chủ
├── Sản phẩm
│   ├── Áo thể thao
│   ├── Quần thể thao
│   ├── Giày
│   └── Phụ kiện
├── Chi tiết sản phẩm
├── Giỏ hàng
├── Thanh toán
├── Đơn hàng
├── Đăng nhập
├── Đăng ký
│
└── Admin
    ├── Dashboard
    ├── Sản phẩm
    ├── Danh mục
    ├── Đơn hàng
    ├── Khách hàng
    ├── Kho hàng
    ├── Khuyến mãi
    └── Báo cáo
```

---

## 🤝 Đóng góp

Nếu muốn đóng góp cho project:

```bash
git checkout -b feature/new-feature

git add .

git commit -m "feat: add new feature"

git push origin feature/new-feature
```

Sau đó tạo **Pull Request**.

---

## 📄 License

Project được xây dựng cho mục đích học tập, nghiên cứu và phát triển thương mại điện tử.

---

## 👨‍💻 Tác giả

**Tên:** Đỗ Minh Quân

**Email:** [dominhquan83866789@gmail.com](mailto:dominhquan83866789@gmail.com)

**GitHub:** `https://github.com/DoMinhQuan8386`

---

## ⭐ Future Features

Các tính năng có thể phát triển thêm:

* [ ] Thanh toán online.
* [ ] Đăng nhập Google.
* [ ] Đăng nhập Facebook.
* [ ] Wishlist / yêu thích sản phẩm.
* [ ] So sánh sản phẩm.
* [ ] Chat hỗ trợ khách hàng.
* [ ] Thông báo đơn hàng.
* [ ] Mã QR cho đơn hàng.
* [ ] Theo dõi vận chuyển.
* [ ] Hệ thống đánh giá sản phẩm.
* [ ] AI hỗ trợ tư vấn sản phẩm.
* [ ] Thống kê doanh thu nâng cao.
