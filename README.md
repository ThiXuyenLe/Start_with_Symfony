# Start_with_Symfony
## 1. Doctrine
- set URL because of company netzwork:
http_proxy...
## 2. Error Limit
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
