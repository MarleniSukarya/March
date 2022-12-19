
# Ujian Akhir Semester 
<br>Mata Kuliah  : Dasar Pemprograman
<br> Nama  : Marleni Sukarya
<br> NIM  : 1227050069
<br>Jurusan  :[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
2. PROGRAM ELEMEN MATRIKS YANG BISA DI BAGI 3,5 ATAU 7
Matriks adalah sekumpulan bilangan yang disusun berdasarkan baris dan kolom, serta ditempatkan di dalam tanda kurung. Baris susunannya horizontal atau ke samping, sedangkan kolom susunannya vertikal atau dari atas ke bawah. Matriks itu punya ukuran. Ukuran matriks disebut ordo. Ordo matriks ini berdasarkan dari banyaknya baris dikali banyaknya kolom pada matriks. Jadi, kalo suatu matriks A memiliki m baris dan n kolom, maka matriks A tersebut berukuran (berordo) m x n. Banyaknya nilai pada matriks di sebut dengan elemen.

Elemen pada matriks tergantung degan nilai yang kita inputkan. Pada artikel ini akan membahan program dimana elemen pada matriks yang dapat dibagi dengan 3,5 atau 7. Pembagian elemen menggunakan operasi matematika pembagian.

Program di buat menggunakan bahasa pemprograman C++. Agar memudahkan dalam meyimpan data yang banyak yang sudah dikelompokan menggunakan Array.

Array adalah kumpulan-kumpulan variabel yang menyimpan data dengan tipe yang sama atau data-data yang tersusun secara linear dimana di dalamnya terdapat elemen dengan tipe yang sama. Indeks dalam array menyatakan elemen yang disimpan dan panjang atau length menyatakan total elemen yang tersimpan.

Indeks dari elemen array dimulai dari 0, bukan 1. Dalam array, untuk membedakan satu variabel dengan variabel lain berdasarkan subscript, bilangan dalam kurung siku […] disebut subscript, dengan subscript masing-masing elemen dapat diakses.

Dalam menyusun fungsi array ada tiga struktur, yaitu kumpulan data dengan tipe sama, gunakan indeks untuk mengakses setiap elemen, dan simpan di tempat yang bersambungan.

## Source Code

```
#include <iostream>
using namespace std;
int main(){
	
	cout<<endl;
	cout<<" Nama	: Marleni Sukarya"<<endl;
	cout<<" NIM	: 1227050069"<<endl;
	cout<<" ================================ "<<endl<<endl;
    
		int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;
	
	    cout<<" Input jumlah baris: "; cin>>jumlahBaris;
	    cout<<" Input jumlah kolom: "; cin>>jumlahKolom;
	    cout << endl;
	
	    for(i = 0; i < jumlahBaris; i++){
	        for(j = 0; j < jumlahKolom; j++){
	            cout << " Baris " <<i+1<<", kolom "<<j+1<< " = ";
	            cin >> arr[i][j];
	        }
	        cout << endl;
	    }
	
	    cout << " Hasil input nilai : " << endl;
	
	    for(i = 0; i < jumlahBaris ; i++){
	    for(j = 0; j < jumlahKolom; j++){
	        cout << setw(3) << arr[i][j] << " ";
	    }
	    cout << endl;
	    }
	
	    cout << "\n Hasil bilangan yang bisa dibagi 3,5 atau 7 : " << endl;
	
	    for(i = 0; i < jumlahBaris ; i++){
	    for(j = 0; j < jumlahKolom; j++){
	        if(arr[i][j] % 3 == 0 || arr[i][j] % 5 == 0 || arr[i][j] % 7 == 0){
	        cout << setw(3) << arr[i][j] << " ";
	        }
	    }
	    cout << endl;
	    }

    
    cout << endl;
    return 0;
}
```


## Output

![ss bagi](https://user-images.githubusercontent.com/120997735/208384707-fa519125-d227-4c7a-ba56-b30f39730ffb.png)



