# Symfony
## 1. Doctrine
- set URL because of company netzwork:

http_proxy...

- dont need to set URL at home


Composer – một trình quản lý dependecy hữu dụng và đơn giản cho PHP. Nó sẽ sắp xếp hợp lý các dependicies của dự án vào một nơi duy nhất.
Composer là công cụ quản lý các thư viện của PHP, bạn cần cài đặt trước khi sử dụng.Composer là một Dependency Management trong PHP, công cụ quản lý các thư viện mà project của bạn sử dụng, bạn chỉ cần khai báo nó, composer sẽ tự động tải code của các thư viện, tạo ra các file cần thiết vào project của bạn, và update các thư viện nếu cần. Composer về bản chất là một cách để đưa tất cả các thư viện, class, file... của 1 bên thứ 3 như CSS frameworks, jQuery plugins và những thứ khác vào project của bạn. Composer được gọi là Dependency management, nghĩa là nó giúp bạn quản lý các thư viện, nhưng không giống như Yum hoặc Apt trong linux, nó không cho các project của bạn dùng chung một đoạn code của thư viện, mà ở mỗi project, nó sẽ tải code của thư viện về và inject vào thư mục gốc trong project của bạn, và bạn hoàn toàn được auto update các thư viện và sử dụng cho project.

Composer là gì?
Composer là một công cụ quản lý các Dependency (bạn có thể hiểu là các thư viện mà chỉ dự án của bạn sử dụng - không dùng bởi nhiều dự án) trong PHP. Vậy Composer quản lý thư viện dựa trên từng Project PHP riêng biệt của bạn, nó cài đặt các thư viện này vào một thư mục có tên vendor trong dự án (mỗi dự án có một thư mục vendor). Composer tự động sinh ra file vendor/autoload.php, từ file này giúp bạn nạp các thư viện đã cài đặt (Nó áp dụng cơ chế tự động nạp theo chuẩn PSR-4 Autoloader) và cả PSR-0 (lỗi thời).

Lợi ích khi sử dụng Composer
Nói chung là các dự án PHP ngày nay là không thể thiếu Composer, vì chúng thường sử dụng rất nhiều loại thự viện. Nếu cài đặt thư viện thủ công thật sự là ác mộng (tích hợp, cập nhật cực cừ mệt mỏi). Khi có Composer dùng thư viện nào chỉ việc khai báo hay gõ tích hợp, khi cập nhật thự viện nào đó, nó cũng tự động giúp bạn cập nhật luôn các thư viện khác mà thư viện cập nhật dùng tới.

Link: https://viblo.asia/p/quan-li-cac-thu-vien-php-voi-composer-7rVRqpr9v4bP
- package/library

Link : https://packagist.org/packages/doctrine/orm

*search: doctrine/orm*

-->  mỗi package có dạng: *vendor/package [phpunit/php-timer]*

This is also called the namespace. The namespace has to be unique for each package on Packagist, as it is used to identify different packages. *Đây là một tin về namespace. Namespace độc nhất cho mỗi package của Packagist, như nó được dùng để xác định các package khác nhau.*

## 1.1 **thông tin tóm tắt**

- lập trình hướng đối tượng OOP, tương tác với các thành phần cơ sở dữ liệu thông qua Model, là các đối tượng thông qua các Class

- CSDL:cơ sở dữ liệu quan hệ/MySQL: lưu dữ liệu theo bản ghi, record: bảng/table, dòng/row

--> kĩ thuật chuyển đổi nhờ ORM: từ dòng, record/Database --> Model/Class kết nối với CSDL, và tạo ra các mqh với nhau nhờ CRUD

ORM tương tác với CSDL--> Doctrine ORM
- các lớp đối tượng trong PHP mà cta sử dụng để tương tác với CSDL thông qua Doctrine --> thực thể /Entity --> mô tả thông tin tương ứng với các bảng CSDL trong database. 4 cách khai báo **Entity**:

-- Docblock Annotations
-- XML
-- YAML
-- PHP Code
**Entity**

* ./bin/console make:entity *

- entity: a normal class that i can save to the database


PS C:\composer> composer require doctrine/orm

## 2. Error Limit: 
Link: https://ourcodeworld.com/articles/read/816/how-to-solve-composer-install-update-error-virtualalloc-failed-0x00000008

 composer require doctrine/orm
 
- **check Limit**: 

php -r "echo ini_get('memory_limit').PHP_EOL;" 

- Solution 1:
//xampp --> php --> php.ini 


*memory_limit = -1* // Use -1 for unlimited(unbegrenzt) or define an explicit value like 2G 

This solution is suggested only for you local machine setup, not suggested for production environment.???
- Solution 2: change PHP to 64 bit !!!
make //new
generate //old

## 3.

Symfony Framework cho phép nhà phát triển tạo các plugin gọi là Gói /bundle/ . Mọi thứ đều là một gói trong Symfony, bao gồm cả chức năng khung lõi và mã được viết cho ứng dụng của bạn.

https://symfony.com/doc/3.4/bundles.html

##4. cấu trúc thư mục
app/config - Chứa tất cả các cấu hình được xác định cho mọi môi trường
app/Resources - Chứa tất cả các mẫu và tệp dịch cho ứng dụng
bin - Chứa các tập tin thực thi
src/AppBundle - Chứa tất cả mã dành riêng cho Symfony (bộ điều khiển và tuyến đường), mã miền của bạn (ví dụ: các lớp học thuyết) và tất cả logic kinh doanh của bạn
tests/AppBundle - Chứa tất cả các bài kiểm tra của ứng dụng
var/cache - Chứa tất cả các tệp bộ đệm được tạo bởi ứng dụng
var/logs - Chứa tất cả các tệp nhật ký được tạo bởi ứng dụng
var/sessions - Chứa tất cả các tệp phiên được tạo bởi ứng dụng
vendor - Chứa tất cả các phụ thuộc ứng dụng được cài đặt bởi Trình soạn thảo
web - Chứa tất cả các tệp của bộ điều khiển phía trước và tất cả các tài sản web, chẳng hạn như bảng định kiểu, tệp JavaScript và hình ảnh.





