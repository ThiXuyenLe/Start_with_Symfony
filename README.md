# Start_with_Symfony
## 1. Doctrine
- set URL because of company netzwork:
http_proxy...
## 2. Error Limit
 composer require doctrine/orm
 
- **check Limit**: 
php -r "echo ini_get('memory_limit').PHP_EOL;" 

//xampp --> php --> php.ini 

; Use -1 for unlimited or define an explicit value like 2G 

*memory_limit = -1*

//-1: unlimited(unbegrenzt) 

Composer – một trình quản lý dependecy hữu dụng và đơn giản cho PHP. Nó sẽ sắp xếp hợp lý các dependicies của dự án vào một nơi duy nhất.

- package/library
Link : https://packagist.org/packages/doctrine/orm

search: doctrine/orm

-->  mỗi package có dạng: *vendor/package [phpunit/php-timer]*

This is also called the namespace. The namespace has to be unique for each package on Packagist, as it is used to identify different packages. *Đây là một tin về namespace. Namespace độc nhất cho mỗi package của Packagist, như nó được dùng để xác định các package khác nhau.*

* thông tin tóm tắt*
-lập trình hướng đối tượng OOP, tương tác với các thành phần cơ sở dữ liệu thông qua Model, là các đối tượng thông qua các Class
-CSDL:cơ sở dữ liệu quan hệ/MySQL: lưu dữ liệu theo bản ghi, record: bảng/table, dòng/row
--> kĩ thuật chuyển đổi nhờ ORM: từ dòng, record/Database --> Model/Class kết nối với CSDL, và tạo ra các mqh với nhau nhờ CRUD

ORM tương tác với CSDL--> Doctrine ORM
- các lớp đối tượng trong PHP mà cta sử dụng để tương tác với CSDL thông qua Doctrine --> thực thể /Entity --> mô tả thông tin tương ứng với các bảng CSDL trong database. 4 cách khai báo Entity:
-- Docblock Annotations
-- XML
-- YAML
-- PHP Code






