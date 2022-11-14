## Writing Test FE Bootcamp Week 3
Nama : Muhammad Arya Wirawan     
Track : Front End Web Development      
Group Track : 2      
Mentor : Thoriq Nur Faizal

### React Context
React Context menyediakan cara untuk berbagi data melalui component tree tanpa harus memberikan props kepada component dibawahnya secara manual di setiap levelnya. Fungsi context mirip dengan redux. Tujuannya yaitu untuk menghindari props drilling yang dalam.

Context didesain untuk membagikan data global untuk component-component dibawahnya. Contohnya seperti auth user, tema, preferensi bahasa dan lain-lain.      
Data yang bersifat global dapat kita simpan dalam context.

#### Membuat Context

Pertama, kita buat terlebih dahulu component context yang akan kita gunakan.    
Selanjutnya, kita dapat membuat context seperti berikut ini:            
![Alt text](asset/createcontext.png)     

Setelah itu, kita panggil contextnya dan kita tambahkan provider
![Alt text](asset/contextprovider.png)

Setelah itu, kita buat state yang berisikan data nilai yang kita inginkan. kemudian kita tambahkan ke value provider
![Alt text](asset/keranjangcount.png)        

Component context akan memprovide data untuk komponen dibawahnya.
![Alt text](asset/propscomponent.png)      
 
Children akan berisikan App.js yang mana di dalam App.js terdapat banyak komponen. Nantinya, context akan memprovide data yang dibutuhkan oleh komponen-komponen tersebut
![Alt text](asset/providerapp.png)    

Setelah itu, kita bungkus App dengan component yang telah kita buat tadi

#### Mengambil data dari context
Untuk mengambil data dari context, kita dapat menggunakan useContext()
![Alt text](asset/usecontexat.png)

Agar context dapat menyebarkan beberapa data, kita dapat melakukannya dengan cara:
![Alt text](asset/123.png)     
Kita share data dengan membungkusnya dengan object. Untuk mengambil datanya, kita dapat destruktur data yang diberikan oleh context diatas
![Alt text](asset/keranjangcoundestruk.png)     
### React Context - Use Reducer      

### React Testing