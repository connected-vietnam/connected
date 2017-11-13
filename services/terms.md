# Terms

### Component
* Là 1 thành phần cơ bản để xây dựng nên trang web.
* Ví dụ về Component:
  * **Navigation**
  * **PostCard**
  * **PostCardList**
* 1 **Component** có thể chứa nhiều **Component** khác, đề làm nên 1 **Component** lớn hơn.
* Ví dụ về kết hợp **Component**:
  - 1 **PostCardList** sẽ gồm nhiều **PostCard**
  - 1 **Navigation** sẽ gồm nhiều **NavigationItem**, 1 **ContactButton**

### Layout
Còn có tên gọi khác là Template
* Bao gồm: Những components được sử dụng lặp đi lặp lại trên 1 số / tất cả các **Page**. Ví dự: Navigation, Footer, Sidebar, ...
* 1 Website có thể có nhiều Layout. Tuy nhiên, 1 Page chỉ có thể sử dụng 1 Layout
* Ví dụ: 1 trang web có 2 kiểu Layout là: có, hoặc không có hiển thị Sidebar

### Page
#### Bao gồm
* Url. VD: https://connected.com.vn
* Layout.
* Những thành phần liên quan đến SEO
  * Meta Tags
  * Title / Description
* Phần nội dung: được đọc lên từ **database**, có thể là 1 bài viết chi tiết, hoặc danh sách các bài viết
* Ví dụ:
  - https://connected.com.vn: Trang chủ (tiếng Việt **Language** = vi)
  - https://connected.com.vn/bai-viet: Trang danh sách bài viết (tiếng Việt **Language** = vi)
  - https://connected.com.vn/bai-viet/3-ly-do-website-nen-co-https: Trang chi tiết bài viết (tiếng Việt **Language** = vi)
  - https://connected.com.vn/en: Trang chủ (tiếng Anh **Language** = en)
  - https://connected.com.vn/posts: Trang danh sách bài viết (tiếng Anh **Language** = en)
  - https://connected.com.vn/post/how-to: Trang chi tiết bài viết (tiếng Anh **Language** = en)

### Content Type
* Phần lưu trữ nội dung bên dưới, dùng để render ra các Component
![Component bất động sản](/images/component-bat-dong-san.png "Component bất động sản")

### Field

### Language

### Theme

### Website
Thông thường 1 website sẽ bao gồm:
* Nhiều **Page**
* 1 hoặc nhiều **Layout**
* 1 hoặc nhiều **Language**
* 1 hoặc nhiều **Theme**. Tuy nhiên trong đồng thời 1 lúc chỉ sử dụng được 1 **Theme** duy nhất
* 1 sitemap.xml
