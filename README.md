# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemograman
<br> Nama		: Septian Hadi Nugroho
<br>NIM			: 1227050122
<br>Jurusan		: [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Di dalam repository ini terdapat 2 program. Pertama, program input banyaknya baris dan kolom lalu menukar kolom jadi baris dan baris jadi kolom (transpose). Kedua, buat pada array 2 dimensi, angka angka diinputkan lalu menampilkan bilangan yang habis dibagi 3, 5, dan 7.
	
## Source Code
 ```c++
 code
```
	#include <iostream>
	using namespace std;

	int main()
	{
		int A[50][50];
		int baris, kolom, i, j, t;
		cout << "===============================" << endl;
		cout << "Nama\t : Septian Hadi Nugroho" << endl;
		cout << "NIM\t : 1227050122" << endl;
		cout << "Kelas\t : IF-C" << endl;
		cout << "===============================" << endl;
		cout << "\tUAS Dasar Pemograman" << endl;
		cout << "\t~~~~~~~~~~~~~~~~~~~~" << endl << endl;

		cout << "Masukkan jumlah baris : ";
		cin >> baris;
		cout << "Masukkan jumlah kolom : ";
		cin >> kolom;

		cout << endl;

	    for(i=0; i<=baris-1; i++)
	    {
		for(j=0; j<=kolom-1; j++)
		{
		    cout << "Masukan nilai baris ke-" << i+1 << " kolom ke-" << j+1 << ": ";;
		    cin >> A[i][j];
		}
		}
		cout << "\nHasil :\n";
	    for(i=0; i<=baris-1; i++)
	    {
		for(j=0; j<=kolom-1; j++)
		{
		    cout << A[i][j] << " ";
		}
		cout << "\n";
		}
		cout << "\nSoal Nomor 1";
		cout << "\nHasil yang sudah ditukar :\n";
	    for(i=0; i<=kolom-1; i++)
	    {
		for(j=0; j<=baris-1; j++)
		{
			cout << A[j][i] << " ";
		}
		cout << "\n";
	    }
	    cout << "\nSoal Nomor 2";
	    cout << "\nHasil yang habis dibagi 3, 5 dan 7 :\n";
	    for(i=0; i<=baris-1; i++)
	    {
		for (j=0; j<=kolom-1; j++)
		{
			if (A[j][i] %3 == 0 && A[j][i] %5 == 0 && A[j][i] %7 == 0)
			{
				cout << A[j][i] << " adalah angka yang habis dibagi 3, 5 dan 7" << endl;
				}
				else
				{
					cout << A[j][i] << " adalah angka yang tidak habis dibagi 3, 5 dan 7" << endl;
				}
			}
		}
		return 0;
	}

## Output
![UAS Dasprog](https://github.com/septianhadinugroho/UAS-Dasprog-Soal/blob/main/uas%20dasprog.PNG)
