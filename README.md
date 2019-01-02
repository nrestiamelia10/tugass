#include <iostream>
#include <cstdlib>
using namespace std;
int main()
{
    float a,b;
    int kode;

    menu:
        cout<< " Kalkulator sederhana C++\n";
        cout<< " Pilihan menu :\n";
        cout<< " 1. Penjumlahan (+)\n";
        cout<< " 2. Pengurangan (-)\n";
        cout<< " 3. Perkalian (:)\n";
        cout<< " 4. Pembagian (x)\n";
        cout<< " Silahkan masukkan kode menu :";cin>>kode;
        if (kode> 4)
        {
            cout<< " \n Kode yang anda masukkan salah silahkan masukkan ulang kode.";
            system("pause");
            system("cls");
            goto menu;
        }
        else
        {
            cout<< " Masukkan angka pertama :";cin>>a;
            cout<< " Masukkan angka kedua :"; cin>> b;
            if (kode==1)
            {
                cout<< "Hasil penjumlahan adalah :"<<a+b<<endl;
            }
            else if (kode==2)
            {
                cout<< "Hasil pengurangan adalah :"<<a-b<<endl;
            }
            else if (kode==3)
            {
                cout<< "Hasil perkalian adalah :"<<a*b<<endl;
            }
            else if (kode==4)
            {
                cout<< " Hasil pembagian adalah :"<<a/b<<endl;
            }
        }
}
