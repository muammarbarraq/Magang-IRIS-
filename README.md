# Rangkuman Pembelajaran Pointer 

Apa itu pointer ?


![pointers](https://user-images.githubusercontent.com/82454139/114570668-3a322f80-9ca0-11eb-8ae0-e3d84bc199b3.png)

## pengertian pointer

Pointer bisa dikatakan sebagai sebuah variabel atau object yang menunjuk ke variabel atau object lainnya.


![reference_operator](https://user-images.githubusercontent.com/82454139/114793048-bc5f4880-9db3-11eb-80cf-fea45df88e8b.png)


![image](https://user-images.githubusercontent.com/82454139/114793134-eca6e700-9db3-11eb-96af-38d5dab2274d.png)

### a. Operator Deference (&)
Operator ini biasanya disebut dengan address of atau operator alamat. Dengan menggunakan operator deference (&) ini, suatu variabel akan menghasilkan alamat memori.

Contoh:
```
int x = 43;
cout << &x;
```
```
#include <iostream>

using namespace std;

int main(){
      int angka = 90;
      int *angkax;
      angkax = &angka;

     cout<<"Nilai (isi) dari variabel angka : "<<angka;
     cout<<"\nAlamat variabel angka (&angka) : "<<&angka;
     cout<<"\nNilai yang ditunjuk pointer *angkax : "<<*angkax;

     return 0;
}
```
*OUTPUT
```
Nilai (isi) dari variabel angka : 90
Alamat variabel angka (&angka) : 0x6ffe34
Nilai yang ditunjuk pointer *angkax : 90
```
![image](https://user-images.githubusercontent.com/82454139/114815299-21309800-9de0-11eb-913c-75f13c70679b.png)


https://1.bp.blogspot.com/-r0Qzgd3sCRA/WDxJeVqXYXI/AAAAAAAAAHU/qbJwq8ciKTQl1E2AtaPA5FFDyr-kaKDZQCLcB/s640/Contoh%2BPenggunaan%2BOperator%2BDereference%2B%2528%2526%2529.PN


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

Dapat dikatakan kalau pointer tidak berisi nilai data, melainkan berisi suatu alamat memori. Lokasi memori tersebut bisa diwakili sebuah variabel atau juga berupa alamat memori secara langsung.

