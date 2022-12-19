# Ujian Akhir Semester 
<br>Mata Kuliah  : Dasar PEmprograman
<br> Nama  : Marleni Sukarya
<br> NIM  : 1227050069 
<br> Jurusan  :[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
    1. PROGRAM TRANSPOSE MATRIKS
    
Matriks adalah sekumpulan bilangan yang disusun berdasarkan baris dan kolom, serta ditempatkan di dalam tanda kurung. Baris susunannya horizontal atau ke samping, sedangkan kolom susunannya vertikal atau dari atas ke bawah. Matriks itu punya ukuran. Ukuran matriks disebut ordo. Ordo matriks ini berdasarkan dari banyaknya baris dikali banyaknya kolom pada matriks. Jadi, kalo suatu matriks A memiliki m baris dan n kolom, maka matriks A tersebut berukuran (berordo) m x n. Banyaknya nilai pada matriks di sebut dengan elemen.
Transpose matriks adalah matriks baru yang diperoleh dengan cara menukar elemen-elemen baris menjadi elemen kolom atau sebaliknya. Pada artikel ini akan dibuatnya program membuat transpose matriks. Program ini menggabungkan antara matematika dan teknologi.
Program di buat menggunakan bahasa pemprograman C++. Agar memudahkan dalam meyimpan data yang banyak yang sudah dikelompokan menggunakan Array. 
Array adalah kumpulan-kumpulan variabel yang menyimpan data dengan tipe yang sama atau data-data yang tersusun secara linear dimana di dalamnya terdapat elemen dengan tipe yang sama. Indeks dalam array menyatakan elemen yang disimpan dan panjang atau length menyatakan total elemen yang tersimpan.
Indeks dari elemen array dimulai dari 0, bukan 1. Dalam array, untuk membedakan satu variabel dengan variabel lain berdasarkan subscript, bilangan dalam kurung siku […] disebut subscript, dengan subscript masing-masing elemen dapat diakses.
Dalam menyusun fungsi array ada tiga struktur, yaitu kumpulan data dengan tipe sama, gunakan indeks untuk mengakses setiap elemen, dan simpan di tempat yang bersambungan.
    
## Source Code

```
#include <iostream>
using namespace std;

int main(void)
{
	system("Color B");
	cout<<endl;
	cout<<" Nama	: Marleni Sukarya"<<endl;
	cout<<" NIM	: 1227050069"<<endl;
	cout<<" ================================ "<<endl<<endl;
	
		int a[10][10]; 
		int transpose[10][10];
		int row;
		int column;
		int i;
		int j;
		
			cout<<" Masukan Baris : ";
			cin>>row;
			cout<<" Masukan Kolom : ";
			cin>>column;
			cout<<" Masukan Elemen Matriks : "<<endl;
			
				// Storing matrix elements
   				for (int i = 0; i < row; ++i) {
    				for (int j = 0; j < column; ++j) {
    				cout << " Masukan Elemen a" << i + 1 << j + 1 << ": ";
         			cin >> a[i][j];
      				}
   				}

   				// Printing the a matrix
				cout << "\n Matrix: " << endl;
				for (int i = 0; i < row; ++i) {
					for (int j = 0; j < column; ++j) {
						cout << " " << a[i][j];
        				if (j == column - 1)
            			cout << endl << endl;
    				}
				}

   				// Computing transpose of the matrix
   				for (int i = 0; i < row; ++i)
    				for (int j = 0; j < column; ++j) {
    				transpose[j][i] = a[i][j];
    			}

   				// Printing the transpose
   				cout << "\n Transpose  Matrix: " << endl;
   				for (int i = 0; i < column; ++i)
    			for (int j = 0; j < row; ++j) {
    			cout << " " << transpose[i][j];
        		if (j == row - 1)
        		cout << endl << endl;
      }

   return 0;
}

```

## Output
	
![SS transpose](https://user-images.githubusercontent.com/120997735/208379758-ab0bdfa1-1b70-46e0-bb63-43329631226b.png)

