# Ujian Akhir Semester 1 
<br>Mata Kuliah 	:Dasar Pemograman
<br> Nama		:Ghani Husna Darmawan
<br>NIM		:	1227050051
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Array dua dimensi adalah sebutan untuk array yang penomoran index-nya menggunakan 2 buah angka. Analogi lain adalah matriks. Matrixs Merupakan kumpulan-kumpulan bilangan yang disusun secara baris (vertikal) dan kolom (horizontal) bisa disebut juga array dua dimensi (multi-dimensional). Transpose Matriks adalah memperoleh sebuah matriks dengan cara menukar baris menjadi kolom dan kolom menjadi baris dari sebuah matriks. Dalam matematika, matriks terdiri dari kolom dan baris. Kembali, untuk menentukan nilai dari sebuah matriks, kita harus sebut secara berpasangan seperti baris 1 kolom 1, atau baris 2 kolom 3, dst. Konsep seperti inilah yang menjadi dasar dari array 2 dimensi. Untuk membuat array 2 dimensi di dalam bahasa C++, caranya tulis 2 kali tanda kurung siku setelah nama variabel, seperti contoh berikut:
int arr[2][2];
Untuk UAS kali ini kami diminta membuat 2 buah program yaitu program pertama adalah membuat array 2 dimensi dengan baris , kolom dan nilai nya di input lalu ditukarkan antara kolom dan baris sedangkan program ke dua digunakan untuk mencari nilai yang dapat di bagi 3, 7, dan 5.
## Source Code 1
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
## Source Code 2
    #include <iostream>
#include <iomanip>
using namespace std;
int main(){
    
    cout << " ===========================" << endl;
    cout << " Ghani Husna Darmawan" << endl;
    cout << " 1227050051 " << endl;
    cout << " ===========================" << endl;
    cout << "\n";
    cout << " === Program bilangan habis dibagi 3,5,7 === " << endl;
    cout << endl;
	int arr[50][50], jumBaris, jumKolom, i, j, baris, kolom;

    cout<<" Input jumlah baris: "; 
	cin>>jumBaris;
    cout<<" Input jumlah kolom: "; 
	cin>>jumKolom;
    cout << endl;

    for(i = 0; i < jumBaris; i++){
        for(j = 0; j < jumKolom; j++){
            cout << " Baris " <<i+1<<", Kolom "<<j+1<< " = ";
            cin >> arr[i][j];
        }
        cout << endl;
    }

    cout << " Hasil input nilai : " << endl;

    for(i = 0; i < jumBaris ; i++){
    for(j = 0; j < jumKolom; j++){
        cout << setw(3) << arr[i][j] << " ";
    }
    cout << endl;
    }

    cout << " Hasil bilangan yang habis dibagi 3,5,7 : " << endl;

    for(i = 0; i < jumBaris ; i++){
    for(j = 0; j < jumKolom; j++){
        if(arr[i][j] % 3 == 0 || arr[i][j] % 5 == 0 || arr[i][j] % 7 == 0){
        cout << setw(3) << arr[i][j] << " ";
        }
    }

    }
    cout << endl;
}
## Output 1
![2022-12-19 (3)](https://user-images.githubusercontent.com/120998349/208375251-dddb318b-63c8-4c3a-abd4-d995c064f158.png)
## Output 2
![2022-12-19 (4)](https://user-images.githubusercontent.com/120998349/208379744-0f7a4c1e-2c70-4ea6-b7ef-b543baf72868.png)
