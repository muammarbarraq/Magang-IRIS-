# Rangkuman Pembelajaran Pointer 

Apa itu pointer ?


![pointers](https://user-images.githubusercontent.com/82454139/114570668-3a322f80-9ca0-11eb-8ae0-e3d84bc199b3.png)

## pengertian pointer

Pointer bisa dikatakan sebagai sebuah variabel atau object yang menunjuk ke variabel atau object lainnya.Jadi pointer tidak berisi nilai data, melainkan berisi suatu alamat memori. Lokasi memori tersebut bisa diwakili sebuah variabel atau juga berupa alamat memori secara langsung.


![reference_operator](https://user-images.githubusercontent.com/82454139/114793048-bc5f4880-9db3-11eb-80cf-fea45df88e8b.png)


![image](https://user-images.githubusercontent.com/82454139/114793134-eca6e700-9db3-11eb-96af-38d5dab2274d.png)

### a. Operator Deference (&)
Operator ini biasanya disebut dengan address of atau operator alamat. Dengan menggunakan operator deference (&) ini, suatu variabel akan menghasilkan alamat memori.

Contoh:
```
int x = 43;
cout << &x;
```
Pada program di atas, akan ditampilkan alamat memori dari variabel x, bukan nilai x.

### b. Operator reference (*)
Operator ini biasanya disebut value pointed by. Dengan menggunakan operator ini, kita dapat mengakses secara langsung nilai yang terdapat pada suatu alamat memori.

Contoh:
```
int x = 76;
cout <<*&x;
```
#### Contoh penerapan pointers 
```
#include <stdio.h>

void main () {

   int  a;
   char b[10];

   printf("Alamat memori variabel a: %x\n", &a);
   printf("Alamat memori variabel b: %x\n", &b);

}
```

Pada program tersebut, kita menggunakan simbol & untuk mengambil alamat memori dari variabel a dan b. Lalu menggunakan format specifier %x untuk menampilkannya dalam bilangan heksadesimal.
* OUTPUTNYA :

![image](https://user-images.githubusercontent.com/82454139/114793841-74d9bc00-9db5-11eb-98e5-8747c03a5622.png)

