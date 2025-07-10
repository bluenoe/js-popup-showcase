# 🧊 Advanced Popup & Modal UI Showcase

<div align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS">
</div>

<div align="center">
  <h3>🎨 Bộ sưu tập các component UI popup đẹp mắt được xây dựng với Tailwind CSS và Vanilla JavaScript</h3>
  <p><em>Một ứng dụng single-page hiện đại showcase các thành phần giao diện người dùng tương tác</em></p>
</div>

---

## ✨ Tính năng nổi bật

### 🎯 **Modals & Dialogs**
- **Standard Modal** - Modal xác nhận chuẩn với overlay và animation
- **Delete Confirmation** - Modal xác nhận xóa với validation input "DELETE"
- **Custom Alert** - Thay thế alert mặc định của browser với thiết kế đẹp

### 🔔 **Notifications & Alerts**
- **Toast Notifications** - 4 loại thông báo (Success, Error, Warning, Info)
- **Auto-dismiss** - Tự động ẩn sau 5 giây
- **Stack Management** - Xếp chồng thông báo một cách gọn gàng

### 🎛️ **Overlays & Panels**
- **Sidebar Panel** - Panel cài đặt trượt từ bên phải
- **User Popover** - Popup thông tin người dùng với menu actions
- **Responsive Design** - Hoạt động mượt mà trên mọi thiết bị

### 🖼️ **Interactive Elements**
- **Tooltip** - Gợi ý hiển thị khi hover
- **Image Lightbox** - Gallery ảnh với navigation và keyboard support
- **Smooth Animations** - Hiệu ứng chuyển động mượt mà

---

## 🚀 Demo trực tiếp

```bash
# Clone repository
git clone <repository-url>

# Chuyển vào thư mục dự án
cd js-popup-showcase

# Khởi chạy server local
python -m http.server 8000
# hoặc
npx serve .

# Mở trình duyệt và truy cập
http://localhost:8000
```

---

## 🏗️ Cấu trúc dự án

```
js-popup-showcase/
├── index.html          # File chính chứa toàn bộ ứng dụng
├── README.md          # Tài liệu dự án
└── assets/            # (Tùy chọn) Thư mục chứa assets bổ sung
```

---

## 🎨 Thiết kế & Công nghệ

### **Frontend Stack**
- **HTML5** - Cấu trúc semantic và accessibility
- **Tailwind CSS** - Framework CSS utility-first
- **Vanilla JavaScript (ES6+)** - Logic tương tác không dependency

### **Design Principles**
- ✅ **Mobile-First Responsive** - Tối ưu cho mọi kích thước màn hình
- ✅ **Accessibility** - Hỗ trợ keyboard navigation và screen readers
- ✅ **Performance** - Single file, load nhanh, không dependencies
- ✅ **Modern UI/UX** - Thiết kế hiện đại với animations mượt mà

---

## 🎯 Các component chi tiết

<details>
<summary><strong>📋 Standard Modal</strong></summary>

- **Mục đích**: Modal xác nhận chuẩn
- **Tính năng**: 
  - Overlay tối với animation fade-in
  - Nút đóng (X) và các action buttons
  - Đóng khi click overlay hoặc ESC
- **Animation**: Scale-up effect
</details>

<details>
<summary><strong>🗑️ Delete Confirmation Modal</strong></summary>

- **Mục đích**: Xác nhận hành động xóa nguy hiểm
- **Tính năng**:
  - Thiết kế màu đỏ cảnh báo
  - Input validation - phải gõ "DELETE" để kích hoạt
  - Disable button cho đến khi validation pass
- **Security**: Ngăn chặn xóa nhầm
</details>

<details>
<summary><strong>🔔 Toast Notifications</strong></summary>

- **Vị trí**: Top-right corner
- **Loại**: Success (xanh), Error (đỏ), Warning (vàng), Info (xanh dương)
- **Tính năng**:
  - Auto-dismiss sau 5 giây
  - Manual close button
  - Stack multiple toasts
- **Animation**: Slide-up effect
</details>

<details>
<summary><strong>⚙️ Settings Sidebar</strong></summary>

- **Vị trí**: Slide từ bên phải
- **Nội dung**: 
  - Toggle switches (Dark mode, Notifications, Auto-save)
  - Dropdown (Language selection)
  - Radio buttons (Theme selection)
- **Animation**: Slide-right với overlay
</details>

<details>
<summary><strong>👤 User Popover</strong></summary>

- **Trigger**: Click button
- **Nội dung**:
  - Avatar và thông tin user
  - Menu actions (Profile, Account, Logout)
- **Positioning**: Dynamic relative to trigger
- **Close**: Click outside hoặc click lại button
</details>

<details>
<summary><strong>🖼️ Image Lightbox Gallery</strong></summary>

- **Trigger**: Click thumbnail images
- **Tính năng**:
  - Full-screen image viewing
  - Previous/Next navigation arrows
  - Keyboard support (←, →, ESC)
  - Close on overlay click
- **Images**: Random Picsum photos
</details>

---

## ⌨️ Keyboard Shortcuts

| Phím | Chức năng |
|------|----------|
| `ESC` | Đóng modal/lightbox hiện tại |
| `←` | Ảnh trước (trong lightbox) |
| `→` | Ảnh tiếp theo (trong lightbox) |
| `Tab` | Navigation accessibility |

---

## 🎨 Customization

### **Màu sắc**
Dự án sử dụng Tailwind CSS color palette. Có thể tùy chỉnh trong các class:
- `bg-blue-600` - Primary buttons
- `bg-red-600` - Danger/Delete actions  
- `bg-green-500` - Success states
- `bg-gray-50` - Background colors

### **Animations**
Các animation được định nghĩa trong `<style>` section:
```css
.fade-in { animation: fadeIn 0.3s ease-out; }
.slide-up { animation: slideUp 0.3s ease-out; }
.scale-up { animation: scaleUp 0.3s ease-out; }
```

### **Responsive Breakpoints**
- `sm:` - 640px+
- `md:` - 768px+
- `lg:` - 1024px+
- `xl:` - 1280px+

---

## 🔧 Browser Support

| Browser | Version |
|---------|--------|
| Chrome | 60+ |
| Firefox | 55+ |
| Safari | 12+ |
| Edge | 79+ |

---

## 📝 License

```
MIT License - Tự do sử dụng cho mục đích cá nhân và thương mại
```

---

## 👨‍💻 Tác giả

**Khanh Blu** - *Frontend Developer*
- 📧 Email: baokhanh.dev281@gmail.com
- 🌐 Portfolio: [Coming Soon]

---

<div align="center">
  <h3>🌟 Nếu project hữu ích, hãy cho một star! 🌟</h3>
  <p><em>Cảm ơn bạn đã xem qua dự án này!</em></p>
</div>

---

## 🔄 Changelog

### v1.1.0 (Latest)
- 🐛 **Fixed**: Lightbox keyboard navigation logic
- ✨ **Improved**: Element visibility state management
- 🎨 **Enhanced**: Animation consistency across components

### v1.0.0
- 🎉 **Initial Release**: Complete popup showcase với 8 components
- 📱 **Responsive**: Mobile-first design
- ♿ **Accessibility**: Keyboard navigation support
- 🎨 **Modern UI**: Tailwind CSS styling

---

<div align="center">
  <sub>Built with ❤️ using Vanilla JavaScript & Tailwind CSS</sub>
</div>