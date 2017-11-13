# Những thông số meta tag cho website Dịch vụ

> Nếu không hiểu meta đó làm gì thì lên đây https://github.com/joshbuchea/HEAD#favicons tìm.
## Tổ chức thành 1 bài viết nói meta là gì, và cách cấu hình nó trên Keystone
## Các meta tag sử dụng
- Common (e.g: title, description, keywords)
  - https://github.com/joshbuchea/HEAD#meta
  - https://github.com/joshbuchea/HEAD#link
  - https://github.com/joshbuchea/HEAD#favicons
- Facebook OpenGraph
- Twitter
## Favicon

Các file cần tạo, **để trên thư mục gốc của Cloudinary**

- favicon-16x16.png
- favicon-32x32.png
- favicon-96x96.png
## Sử dụng riêng cho từng trang
- url (tự động)
- title (tự động cho trang detail)
- description (tự động cho trang detail)
- subject (nên có)
- imageUrl: tự động lấy cho trang detail
- author (lấy tự động, optional, nếu không có sẽ lấy phần cấu hình toàn cục)
- fbAppId (`nên có`, nếu không có sẽ lấy phần cấu hình toàn cục)
- twSiteAccount (nên có, nếu không có sẽ lấy phần cấu hình toàn cục)
- twCreator (nên có, nếu không có sẽ lấy phần cấu hình toàn cục)
- googlePlusPublisher (nên có, nếu không có sẽ lấy phần cấu hình toàn cục)
- meta (là 1 array, cấu hình thêm, sẽ đè lên tất cả các cái còn lại)
## Cấu hình cho toàn site
- siteName (name trong config): Bắt buộc
- subject: chủ đề của website đó nói về gì (optional)
- locale: ngôn ngữ của site (lấy tự động)
- *imageDir*: thông thường sẽ là root path của Cloudinary
- author (tên của người viết bài)
- fbAppId  (nên có)
- twSiteAccount (nên có)
- twCreator (nên có)
- googlePlusPublisher (nên có)
## Cách thức hoạt động
- Những gì liên quan đề title (og:title, twitter:title) sẽ tự động lấy từ title
- Những gì liên quan đề description sẽ tự động lấy từ description

Ví dụ:

    title: Bài viết # Những tag này nếu có sẽ đè lên title, description mặc định của bài viết
    description: Nội dung cơ bản của meta description
    imageUrl:
    meta: # Những tag dưới này sẽ được ưu tiên hàng đầu
    - name: description
      content: Nội dung này sẽ được đè lên cho meta description

Ở ví dụ trên thì:

- `og:description`, `twitter:description` sẽ có giá trị là Nội dung cơ bản của meta description
- còn thẻ meta description là: Nội dung này sẽ được đè lên cho meta description

**Mức độ ưu tiên**

- Trong phần meta
- Trong phần title
- Title / Name / Description mặc định của data
## Check list cấu hình meta tags cho tất cả các trang

VD như trang:
**Home**

- Trang chủ
- Lưu trong Config.meta

**Posts**

- Trang danh sách tất bài viết
- lưu Config.meta

**Post Category**

- Trang danh sách bài viết trong 1 category
- lưu trong meta trong PostCategory

**Post Tag**

- Trang danh sách bài viết trong 1 tag
- lưu trong meta trong PostTag

**Services**

- Trang danh sách dịch vụ
- lưu trong Config.meta

**Service Category**

- Trang danh sách dịch vụ trong 1 Service Category
- lưu trong meta trong ServiceCategory

**Page**

- Trang chi tiết trang
- lưu trong meta trong Page

**Post**

- Trang chi tiết bài viết
- lưu trong meta trong Post

**Contact**

- Trang liên hệ
- lưu trong Config.meta

