: DYNAMIC ROUTE DAN MIDDLEWARE
------------------------------------------------
Langkah 1) Menambahkan syntax dynamic route pada file web.php yang berfungsi untuk memanggil
user berdasarkan ID yang dimasukkan.
Memanggil user dengan ID 9 pada Postman.
Menambahkan syntax dynamic route pada file web.php yang berfungsi untuk mengambil
post dan comment berdasarkan ID yang dimasukkan. Pada syntax ini kita membuktikan
bahwa routes dapat memiliki lebih dari satu parameter.
Memanggil post dengan ID 1 dan comments dengan ID 5 pada Postman
Menambahkan syntax dynamic route pada file web.php yang berfungsi menyajikan
pilihan untuk memanggil seluruh user maupun berdasarkan ID-nya
Memanggil seluruh user pada Postman
Memanggil user berdasarkan ID-nya yaitu 2 pada Postman

<img src="1.jpg">
<img src="2.jpg">
<img src="3.jpg">
<img src="4.jpg">


Langkah 2) Menambahkan syntax aliases route pada file web.php yang berfungsi menampilkan pesan
“Berhasil login”. Mengakses fungsi /auth/login pada Postman
Mengakses endpoint /profile pada Postman. Karena pada langkah sebelumnya telah
diatur menjadi true, maka routes akan memanggil route.auth.login dan menampilkan
pesan seperti pada gambar.

<img src="5.jpg">
<img src="6.jpg">
<img src="7.jpg">
<img src="8.jpg">

Langkah 3) Menambahkan syntax group route pada file web.php.Mengakses prefix /users pada
Postman. Sesuai prefix yang ditentukan pada langkah sebelumnya, maka yang
ditampilkan adalah “GET /users”. Mengakses prefix /users/register pada Postman. Sesuai
prefix yang ditentukan pada langkah sebelumnya, maka yang ditampilkan adalah “GET
/users/test”.

<img src="9.jpg">

Langkah 4) Membuat file AgeMiddleware.php pada direktori app/Http/Middleware, kemudian
menambahkan fungsi handle sesuai yang terdapat pada modul. Fungsi ini berisi
pengondisian dimana jika age < 17, maka akan menjalankan routes /fail.Mendaftarkan
AgeMiddleware pada file bootstrap/app.Menambahkan routes /fail dan middleware pada
routes /admin/home.Mengakses prefix /admin/home pada Postman. Mengakses prefix
/admin/home pada Postman. Mengakses prefix /admin/home pada Postman. Mengakses
prefix /admin/home pada Postman

<img src="10.jpg">
<img src="11.jpg">
<img src="12.jpg">
<img src="13.jpg">

