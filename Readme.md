# Open-closed principle

Open Closed Principle pertama kali diperkenalkan oleh Robert C.Martin pada tahun 1996 dan masih relevan sampai sekarang. Prinsip ini berbunyi sebagai berikut.

SOFTWARE ENTITIES (CLASSES, MODULES, FUNCTIONS, ETC.)
SHOULD BE OPEN FOR EXTENSION, BUT CLOSED FOR
MODIFICATION. 

Memodifikasi bagian-bagian pada pemrograman itu boleh saja, namun beresiko. Resiko yang dimaksud misalnya Anda memodifikasi bagian salah satu fungsi, namun ternyata menimbulkan efek samping terhadap fungsi lain. Resiko ini dapat diminimalisir dengan penerapan prinsip single responsibility dan open/closed principle pada source code yang dibuat. Alih-alih dimodifikasi, sebaiknya bagian-bagian tersebut dirancang supaya extendable atau bisa diperluas kegunaanya.


## Tujuan Program

Untuk menghindari keretakan software dikarenakan perubahan secara langsung terhadap sebuah class, module, ataupun function.

## Tentang Program

- Pada Source Code ini terdapat 2 program, yakni CouponWithOCP dan CouponWithoutOCP
- Pada bagian CouponWithOCP, Kita dapat mengubah object menjadi object lain tanpa harus meninggalkan fungsi sesungguhnya dengan menggunakan Abstraction. Sedangkan pada bagian CouponWithoutOCP, jika kalian mengubah salah satu fungsi maka akan memengaruhi fungsi lain.