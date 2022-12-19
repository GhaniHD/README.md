# Ujian Akhir Semester 
<br>Mata Kuliah 	:Dasar Pemograman
<br> Nama		:Ghani Husna Darmawan
<br>NIM		:	1227050051
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

## Source Code
#include <iostream>
using namespace std;

int main()
{
    cout << " ===========================" << endl;
    cout << " Ghani Husna Darmawan" << endl;
    cout << " 1227050051 " << endl;
    cout << " ===========================" << endl;
    cout << "\n";
    cout << " === Program Perkalian Matrix Ordo 2 === " << endl;
    cout << endl;
    double a[50][50];
    int i, j, k, baris, kolom;

    cout << " masukan baris = ";
    cin >> baris;
    cout << " masukan kolom = ";
    cin >> kolom;
    cout << endl;

    cout << endl
         << " Elemen matriks A : " << endl;
    for (i = 0; i < baris; i++)
    {
        for (j = 0; j < kolom; j++)
        {
            cout << " Baris " <<i<<", Kolom "<<j<< " = ";
            cin >> a[i][j];
             
        }
        cout<<"\n";
    }

    cout << endl;

    cout << " Element matriks A adalah : " << endl;
    for (i = 0; i < baris; i++)
    {
        for (j = 0; j < kolom; j++)
        {
            cout << "    " << a[i][j];
        }
        cout << endl;
    }
    cout << endl;
    cout << endl;
    cout << " Matriks di balik :" << endl;
    for (i = 0; i < kolom; i++)
    {
        
        for (j = 0; j < baris; j++)
        {
            cout << "    " << a[j][i];
        }
        cout << endl;
    }
    return 0;
}
## Output
![2022-12-19 (3)](https://user-images.githubusercontent.com/120998349/208375251-dddb318b-63c8-4c3a-abd4-d995c064f158.png)
