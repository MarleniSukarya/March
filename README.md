# Ujian Akhir Semester 
<br>Mata Kuliah  : Dasar PEmprograman
<br> Nama  : Marleni Sukarya
<br> NIM  : 1227050069 
<br> Jurusan  :[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
    1. PROGRAM TRANSPOSE MATRIKS
            Pembuatan program Transpose Matriks menggunakan bahasa pemprograman C++ dimana ini merupakan Array. Program ini menggabungkan antara matematika dan 
       teknologi.
       
    2. Program Elemen Matriks dimana dapat dibagi dengan 3,5 atau 7
    
## Source Code

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



## Output

