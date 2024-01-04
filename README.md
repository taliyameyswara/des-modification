# DES Modification
Modified DES Algorithm for Generate Key, Encryption and Decryption
#### Taliya Meyswara (A11.2022.14163) - A11.43UG1
> Program ini dibuat untuk memenuhi Tugas Akhir Mata Kuliah Kriptografi

## Detail Modifikasi 🧩
Program ini merupakan modifikasi dari algoritma DES (Data Encryption Standard) dengan detail modifikasinya adalah sebagai berikut: 
| Proses              | Sebelum Modifikasi                                                                                                                                                           | Setelah Modifikasi                                                                                                                                                               |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Generate key        | Kunci yang diinputkan harus 8 karakter                                                                                                                                       | Jika kunci yang diinputkan kurang dari 8 karakter maka akan ditambahkan karakter acak hingga mencapai 8 karakter, jika lebih maka akan dikurangi hingga menjadi 8 karakter        |
| Generate key        | Proses generate kunci biner (menjadi 56 bit) setelah dipermutasi menggunakan tabel pc 1 dibagi menjadi 2 bagian yaitu left (L) dan right (R) dimana masing-masing sepanjang 28 bit | Proses generate kunci biner (menjadi 56 bit) setelah dipermutasi menggunakan tabel pc 1 dibagi menjadi 4 bagian yaitu part1, part2, part3, part4 dimana masing-masing sepanjang 14 bit |
| Enkripsi & Dekripsi | Setelah melakukan proses permutasi dengan tabel IP-1, baris biner tersebut dibagi menjadi 2 bagian, sehingga masing-masing bagian terdapat 32 bit                            | Setelah melakukan proses permutasi dengan tabel IP-1, baris biner tersebut dibagi menjadi 4 bagian, sehingga masing-masing bagian terdapat 16 bit                                |
| Enkripsi & Dekripsi | Tabel fungsi ekspansi e berisi angka 1-32, karena left (L) dan right (R) sama-sama memiliki 32 bit.                                                                          | Tabel fungsi ekspansi e hanya berisi angka 1-16 karena setiap bagian hanya terdapat 16 bit.                                                                                      |
| Enkripsi & Dekripsi | Hasil dari proses S-Box dipermutasikan dengan tabel fungsi p yang berisi 32 sel                                                                                              | Hasil dari proses S-Box dipermutasikan dengan tabel fungsi p yang berisi 16 sel                                                                                                  |

## Cara Menjalankan ✨
1. Clone Repository
  ```git clone https://github.com/taliyameyswara/des-modification.git```
2. Sediakan plaintext berupa gambar (.jpeg)
3. Run all file modified_des.ipynb
4. Masukkan path file yang akan di-encoding (contoh: plaintext.jpeg)
5. Masukkan kunci yang diinginkan
6. Tunggu proses running selesai
7. Cek detail proses dan hasil pada folder yang ada

> [!NOTE]  
> Pastikan sudah setup python environment untuk menjalankan project,\
> atau jalankan melalui google collabs 👇🏻\
> https://colab.research.google.com/drive/1HpyJI4Y02xtbejhevEmURMjKdREp1dek?usp=sharing

&copy; 2024 Taliya Meyswara.
