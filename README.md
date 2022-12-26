# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemograman
<br> Nama		: Septian Hadi Nugroho
<br>NIM		: 1227050122
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

## Source Code

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
    		if (A[i][j] %3 == 0 && A[j][i] %5 == 0 && A[j][i] %7 == 0)
    		{
    			cout << A[i][j] << " adalah angka yang habis dibagi 3, 5 dan 7" << endl;
			}
			else
			{
				cout << A[i][j] << " adalah angka yang tidak habis dibagi 3, 5 dan 7" << endl;
			}
		}
	}
	return 0;
}
## Output

===============================
Nama     : Septian Hadi Nugroho
NIM      : 1227050122
Kelas    : IF-C
===============================
        UAS Dasar Pemograman
        ~~~~~~~~~~~~~~~~~~~~

Masukkan jumlah baris : 2
Masukkan jumlah kolom : 2

Masukan nilai baris ke-1 kolom ke-1: 1
Masukan nilai baris ke-1 kolom ke-2: 2
Masukan nilai baris ke-2 kolom ke-1: 9
Masukan nilai baris ke-2 kolom ke-2: 8

Hasil :
1 2
9 8

Soal Nomor 1
Hasil yang sudah ditukar :
1 9
2 8

Soal Nomor 2
Hasil yang habis dibagi 3, 5 dan 7 :
1 adalah angka yang tidak habis dibagi 3, 5 dan 7
2 adalah angka yang tidak habis dibagi 3, 5 dan 7
9 adalah angka yang tidak habis dibagi 3, 5 dan 7
8 adalah angka yang tidak habis dibagi 3, 5 dan 7

--------------------------------
Process exited after 141.9 seconds with return value 0
Press any key to continue . . .
