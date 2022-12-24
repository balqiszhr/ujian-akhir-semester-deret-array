# Ujian Akhir Semester
<br> Mata Kuliah : Dasar Pemrograman
<br> Nama        : Balqis Salsabillah Azzahra
<br> NIM         : 1227050028
<br> Jurusan     : [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

<br> Kali ini kita akan membuat array dalam implementasi deret aritmatika, untuk mencari bilangan yang tidak habis dibagi dengan angka 3, 5, dan 7.
<br> Algoritma dari Source Code ini yaitu :
<br> 1. User menginputkan jumlah baris pada array dengan range 0-20.
<br> 2. User menginputkan jumlah kolom pada array dengan range 0-20.
<br> 3. User menginputkan nilai tiap baris dan kolom.
<br> 4. Kemudian nilai divalidasi apakah nilai tersebut habis dibagi 3,5 dan 7.
<br> 5. Apabila nilai tadi habis dibagi dengan angka 3,5 dan 7, maka nilai tidak akan ditampilkan.
<br> 6. Apabila tidak habis maka nilai akan ditampilkan.

## Source Code

<br> #include
<br> using namespace std;
<br> int main () {
    <br> int A [20][20];
    <br> int b, k, i, j;
    <br> cout << "Masukkan Jumlah Baris : "; cin >> b;
    <br> cout << "Masukkan Jumlah Kolom : "; cin >> k;

    <br> for (i=0; i<=b-1; i++){
        <br> for (j=0; j<=k-1; j++){
            <br> cout << "Masukkan Nilai : ("<<i+1<<"."<<j+1<<") : "; cin >> A[i][j];
        }
    }
    <br> cout << "Nilai yang diinputkan : \n";
    <br> for (int i=0; i<b; i++){
        <br> for (int j=0; j<k; j++){
            <br> cout << A[i][j]<<"\t";
        }
        <br> cout << endl;
    }
    <br> int angka [20];
    <br> int index=0;
    <br> for (i=0; i<b; i++){
        <br> for (j=0; j<k; j++){
            <br> if (A [i][j]%3 != 0 && A[i][j]%5 != 0 && A[i][j]%7 !=0){
                <br> angka [index] = A[i][j];
                <br> index++;
            }
        }
    }
    <br> cout << "Angka yang tidak habis dibagi dengan 3, 5, dan 7 adalah ";
    <br> for (int i=0; i<index; i++){
        <br> cout << angka[i] << ", ";
    }
}

## Output

![deret](https://user-images.githubusercontent.com/121304572/209416886-a702f520-808f-4ed7-befe-981a0fe751b7.jpg)
