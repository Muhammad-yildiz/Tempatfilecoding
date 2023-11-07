#include <iostream>

int main() {
    int ukuranKotak = 4;  // Ukuran setiap kotak
    int jarakAntarKotak = 1;  // Jarak antara kotak (didekatkan)

    for (int i = 0; i < 3; i++) {  // Baris kotak
        for (int j = 0; j < ukuranKotak; j++) {  // Baris dalam kotak
            for (int k = 0; k < 3; k++) {  // Kotak dalam kolom
                for (int l = 0; l < ukuranKotak; l++) {  // Kolom dalam kotak
                    if (j == 0 || j == ukuranKotak - 1 || l == 0 || l == ukuranKotak - 1) {
                        std::cout << "*";
                    } else {
                        std::cout << " ";
                    }
                }
                std::cout << "  ";  // Jarak antara kotak dalam kolom
            }
            std::cout << std::endl;
        }
        for (int m = 0; m < ukuranKotak; m++) {  // Jarak antara kotak dalam baris
            std::cout << std::endl;
        }
    }

    return 0;
}
