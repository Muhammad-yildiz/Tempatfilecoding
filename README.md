#include <iostream>
using namespace std;
int main() {
    int ukuranKotak = 15;  // Ukuran setiap kotak
    int jarakAntarKotak = 3;  // Jarak antara kotak (didekatkan)

    for (int i = 0; i < 1; i++) {  // Baris kotak
        for (int j = 0; j < ukuranKotak; j++) {  // Baris dalam kotak
            for (int k = 0; k < 1; k++) {  // Kotak dalam kolom
                for (int l = 0; l < ukuranKotak; l++) {  // Kolom dalam kotak
                    if (j == 0 || j == 15 - 11 || l == 0 || l == 15 - 8 || j==0 || j == 15-5 || l == 0 || l == 15-1|| j==0|| j== 15-1) {
                        cout << "*";
                    } else {
                        cout << " ";
                    }
                }
                cout << "  ";  // Jarak antara kotak dalam kolom
            }
            cout << endl;
        }
        for (int m = 0; m < ukuranKotak; m++) {  // Jarak antara kotak dalam baris
            cout <<endl;
        }
    }

    return 0;
}
