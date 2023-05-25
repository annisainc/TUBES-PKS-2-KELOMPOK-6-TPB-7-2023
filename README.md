# Program Tes Kesehatan Mental
Program akan melakukan tes dari pertanyaan yang diberikan dan menghasil poin dari jawaban yang dipilih yang memiliki range masing-masing, kemudian akan ditentukan hasil akhirnya termasuk ke kategori mana.

## Anggota Kelompok
1. Annisa Indah Cahyani	  122430045 Teknik Biomedis
2. Atha Azarine           122430046 Teknik Biomedis
3. Qonita Sholehati Amri  122430048 Teknik Biomedis
4. Salma Anindya Oktrina  122430034 Teknik Biomedis

## Pengantar Komputer & Software
- Nama Dosen: Asep Nurul Ajiid Mustofa, S.T., M.T.
- Nama asisten praktikum 1: Marchel Timoteus
- Nama asistem praktikum 2: David Panondang Sinaga

## Cara Kerja Program
1. Program akan meminta tiga hal (dalam satu kata) yang membuat user bahagia. Menggunakan array, ketiga hal tersebut akan muncul dalam satu baris.
2. Program akan meminta jawaban user dari pertanyaan yang diajukan. Terdapat 4 pilihan jawaban sehingga user memilih angka 1 - 4. Menggunakan percabangan, setiap pilihan pada pertanyaan memiliki poin masing-masing.
3. Program akan meminta jawaban dari 10 pertanyaan.
4. Program akan menjumlahkan total poin dari jawaban user pada pertanyaan ke-1 hingga ke-10. Menggunakan percabangan, jumlah total akan menjadi acuan bahwa hasil tes masuk ke dalam kategori mana.
5. Program menyediakan sebanyak 4 kategori hasil tes.
6. Program mengajukan pertanyaan untuk mengulangi tes atau tidak. Menggunakan perulangan, maka jawaban dari user akan memberikan keputusan untuk mengulangi tes kembali atau tidak.
7. Program selesai dijalankan.

## Cara Menggunakan Program
1. Akses link program running yang tersedia.
2. Jalankan program dengan menekan tombol Run.
3. Masukkan tiga hal yang dapat membuat user bahagia (dalam satu kata sebanyak 3 kali).
4. Masukkan jawaban yang paling sesuai dengan anda melalui pertanyaan yang diajukan program (sebanyak 10 pertanyaan) dengan memilih nomor 1 - 4 karena pada setiap pertanyaan terdapat 4 pilihan jawaban.
5. Akan muncul hasil tes yang telah dilakukan.
6. Masukkan pilihan anda untuk mengulangi program dengan menjawab "ya" atau "tidak".
7. Program selesai dijalankan.

## Media
| File | Link Akses |
| ------ | ------ |
| Laporan | -- |
| Video | -- |
| Program | https://github.com/annisainc/TUBES-PKS-2-KELOMPOK-6-TPB-7-2023/blob/main/README.md |
| Program Running | https://replit.com/@ANNISA-INDAHIND/PROGRAM-TES-KESEHATAN-MENTAL |
| Code Program | https://onlinegdb.com/KKy_hKA8r |

## Kode Program

    #include <iostream>
    using namespace std;

    // Anggota-NIM
    // Annisa Indah Cahyani	  122430045
    // Atha Azarine	          122430046
    // Qonita Sholehati Amri	122430048
    // Salma Anindya Oktrina	122430034

    int main() {
      int pilih1, pilih2, pilih3, pilih4, pilih5, pilih6, pilih7, pilih8, pilih9,
          pilih10;
      int poin1, poin2, poin3, poin4, poin5, poin6, poin7, poin8, poin9, poin10;
      int total, i;
      string pilihan;
      string reason[3];

      do {
        cout << "\nTES KESEHATAN MENTAL/PSIKOLOGI SEDERHANA \n";
        cout << "KELOMPOK 6 TPB 7 2023 PKS 2 \n";
        cout << "-------------------------------------------\n\n";
        cout << "\nSebelum memulai, apa 3 hal (dalam satu kata) yang bisa membuat "
                "anda bahagia? \n";
        for (i = 1; i <= 3; i++) {
          cout << "Hal ke- " << i << " : ";
          cin >> reason[i - 1];
        }
        for (i = 0; i < 3; i++) {
          cout << reason[i] << " ";
        }
        cout << endl;
        cout << "Selalu ingat, bahwa ketiga hal ini bisa memberikan rasa bahagia "
                "pada anda :) = "
             << endl;
        cout << endl;
        cout << "\n-------------------------------------------\n";
        cout << "\nTes Psikologi Sederhana : Pertanyaan 1 \n";
        cout << "-------------------------------------------\n\n";
        cout << "BAGAIMANA PERASAANMU SAAT INI? \n";
        cout << "1. SEDIH\t";
        cout << "2. RESAH/KHAWATIR\n\n";
        cout << "3. KESEPIAN\t";
        cout << "4. SENANG/GEMBIRA\n";
        cout << "\n-------------------------------------------\n";
        cout << "\n\nPilih (1-4): ";
        cin >> pilih1;
        if (pilih1 == 1) {
          poin1 = 4;
        } else if (pilih1 == 2) {
          poin1 = 2;
        } else if (pilih1 == 3) {
          poin1 = 3;
        }
        if (pilih1 == 4) {
          poin1 = 1;
        }

    cout << "\nTes Psikologi Sederhana : Pertanyaan 2 \n";
    cout << "-------------------------------------------\n\n";
    cout << "BAGAIMANA PENDAPAT TEMANMU TENTANG DIRIMU?\n";
    cout << "1. MENYENANGKAN\t\t";
    cout << "2. JUDES ATAU GALAK\n\n";
    cout << "3. SUKA CANGGUNG\t";
    cout << "4. BERSIKAP DINGIN\n";
    cout << "\n-------------------------------------------\n";
    cout << "\n\nPilih (1-4) :";
    cin >> pilih2;
    if (pilih2 == 1) {
      poin2 = 1;
    } else if (pilih2 == 2) {
      poin2 = 4;
    } else if (pilih2 == 3) {
      poin2 = 2;
    }
    if (pilih2 == 4) {
      poin2 = 3;
    }

    cout << "\nTes Psikologi Sederhana : Pertanyaan 3\n\n";
    cout << "-------------------------------------------\n\n";
    cout << "BAGAIMANA SIKAPMU DI DALAM KELUARGA?\n";
    cout << "1. BIASA AJA\t\t";
    cout << "2. PENDIAM\n\n";
    cout << "3. SUKA BERCANDA\t";
    cout << "4. TIDAK TAU\n";
    cout << "\n-------------------------------------------\n";
    cout << "\n\nPilih (1-4) :";
    cin >> pilih3;
    if (pilih3 == 1) {
      poin3 = 3;
    } else if (pilih3 == 2) {
      poin3 = 2;
    } else if (pilih3 == 3) {
      poin3 = 1;
    }
    if (pilih3 == 4) {
      poin3 = 4;
    }

    cout << "\nTes Psikologi Sederhana : Pertanyaan 4\n\n";
    cout << "-------------------------------------------\n\n";
    cout << "APA KAMU SENANG NONGKRONG BARENG?\n";
    cout << "1. HANYA SAMA TEMAN\t";
    cout << "2. YAP,SUKA YANG RAME\n\n";
    cout << "3. LEBIH SENANG SENDIRI\t";
    cout << "4. TIDAK SUKA\n";
    cout << "\n-------------------------------------------\n";
    cout << "\n\nPilih (1-4) :";
    cin >> pilih4;
    if (pilih4 == 1) {
      poin4 = 2;
    } else if (pilih4 == 2) {
      poin4 = 1;
    } else if (pilih4 == 3) {
      poin4 = 3;
    }
    if (pilih4 == 4) {
      poin4 = 4;
    }

    cout << "\nTes Psikologi Sederhana : Pertanyaan 5\n";
    cout << "-------------------------------------------\n\n";
    cout << "KUTIPAN MANA YANG KAMU PILIH?\n";
    cout << "1. HIDUP ITU MEMBOSANKAN\t\t\t";
    cout << "2. HIDUP ITU SEPERTI PERMEN KARET\n\n";
    cout << "3. TEMAN SEJATI SELALU ADA DIMASA SULIT\t";
    cout << "4. HIDUP ITU INDAH\n";
    cout << "\n-------------------------------------------\n";
    cout << "\n\nPilih (1-4) :";
    cin >> pilih5;
    if (pilih5 == 1) {
      poin5 = 3;
    } else if (pilih5 == 2) {
      poin5 = 2;
    } else if (pilih5 == 3) {
      poin5 = 4;
    }
    if (pilih5 == 4) {
      poin5 = 1;
    }

    cout << "\nTes Psikologi Sederhana : Pertanyaan 6\n";
    cout << "-------------------------------------------\n\n";
    cout << "WARNA APA YANG KAMU SUKAI?\n";
    cout << "1. MERAH/KUNING \t\t";
    cout << "2. HIJAU/BIRU \n\n";
    cout << "3. HITAM/ABU-ABU\t";
    cout << "4. PUTIH/LAINNYA \n";
    cout << "\n-------------------------------------------\n";
    cout << "\nPilih (1-4): ";
    cin >> pilih6;

    if (pilih6 == 1) {
      poin6 = 1;
    } else if (pilih6 == 2) {
      poin6 = 4;
    } else if (pilih6 == 3) {
      poin6 = 3;
    }
    if (pilih6 == 4) {
      poin6 = 2;
    }

    cout << "\nTes Psikologi Sederhana : Pertanyaan 7\n";
    cout << "-------------------------------------------\n\n";
    cout << "APA KAMU BISA MENGENDALIKAN EMOSIMU?\n";
    cout << "1. TERGANTUNG SITUASI \t";
    cout << "2. ENTAHLAH \n\n";
    cout << "3. TENTUNYA BISA DONG \t";
    cout << "4. TIDAK BISA \n";
    cout << "\n-------------------------------------------\n";
    cout << "\nPilih (1-4): ";
    cin >> pilih7;

    if (pilih7 == 1) {
      poin7 = 4;
    } else if (pilih7 == 2) {
      poin7 = 3;
    } else if (pilih7 == 3) {
      poin7 = 1;
    }
    if (pilih7 == 4) {
      poin7 = 2;
    }

    cout << "\nTes Psikologi Sederhana : Pertanyaan 8\n";
    cout << "-------------------------------------------\n\n";
    cout << "APA YANG KAMU LAKUKAN DALAM WAKTU LUANG?\n";
    cout << "1. BERFIKIR BANYAK HAL\t";
    cout << "2. MENONTON FILM \n\n";
    cout << "3. MENDENGARKAN MUSIK \t";
    cout << "4. NGOBROL/NONGKRONG \n";
    cout << "\n-------------------------------------------\n";
    cout << "\nPilih (1-4): ";
    cin >> pilih8;

    if (pilih8 == 1) {
      poin8 = 2;
    } else if (pilih8 == 2) {
      poin8 = 3;
    } else if (pilih8 == 3) {
      poin8 = 4;
    }
    if (pilih8 == 4) {
      poin8 = 1;
    }

    cout << "\nTes Psikologi Sederhana : Pertanyaan 9\n";
    cout << "-------------------------------------------\n\n";
    cout << "MANA YANG JADI KEINGINAN KAMU? \n";
    cout << "1. HIDUP BAHAGIA \t\t";
    cout << "2. MENJADI PRIBADI YANG LEBIH BAIK \n\n";
    cout << "3. BISA BERHENTI KHAWATIR \t";
    cout << "4. BERSENANG-SENANG \n";
    cout << "\n-------------------------------------------\n";
    cout << "\nPilih (1-4): ";
    cin >> pilih9;

    if (pilih9 == 1) {
      poin9 = 1;
    } else if (pilih9 == 2) {
      poin9 = 3;
    } else if (pilih9 == 3) {
      poin9 = 2;
    }
    if (pilih9 == 4) {
      poin9 = 4;
    }

    cout << "\nTes Psikologi Sederhana : Pertanyaan 10\n";
    cout << "-------------------------------------------\n\n";
    cout << "BAGAIMANA KAMU MENJALANI KEHIDUPAN KAMU? \n";
    cout << "1. MENGALIR SEPERTI AIR \t\t";
    cout << "2. PENUH TEKANAN \n\n";
    cout << "3. DIPENUHI KEGEMBIRAAN \t";
    cout << "4. TIDAK PEDULI \n";
    cout << "\n-------------------------------------------\n";
    cout << "\nPilih (1-4): ";
    cin >> pilih10;

    if (pilih10 == 1) {
      poin10 = 4;
    } else if (pilih10 == 2) {
      poin10 = 2;
    } else if (pilih10 == 3) {
      poin10 = 1;
    }
    if (pilih10 == 4) {
      poin10 = 3;
    }

    cout << "\nTes Psikologi Sederhana\n";
    cout << "--------------------------------------\n\n";

    total = poin1 + poin2 + poin3 + poin4 + poin5 + poin6 + poin7 + poin8 +
            poin9 + poin10;
    cout << "Poin anda adalah = " << total << endl;

    if (total <= 16) {
      cout << "Anda Tidak Memiliki Gangguan Mental\n\n";
      cout << "Anda selalu menjadi diri anda sendiri. Teruslah bahagia dan "
              "gembira!. \n";
    } else if (total <= 24) {
      cout << "GELISAH \n\n";
      cout << "Sikap anda terlalu serius, membuat anda akan mudah panik saat "
              "menghadapi sesuatu. \n";
      cout << "Cobalah untuk lebih bersantai serta cobalah untuk mulai "
              "mempercayai orang-orang disekitarmu. \n";
    } else if (total <= 32) {
      cout << "ANTI SOSIAL\n\n";
      cout << "Anda merasa gugup saat berada dalam suatu kelompok, sehingga "
              "Anda memilih untuk menyendiri.\n";
      cout << "Hal tersebut disebabkan oleh kurangnya dalam mengungkapkan rasa "
              "empati dan emosi yang Anda alami. \n";
      cout << "Cobalah untuk sering berkomunikasi seperti menyapa keluarga dan "
              "orang-orang terdekatmu. \n";
    } else if (total <= 40) {
      cout << "DEPRESI \n\n";
      cout << "Anda selalu dibebani oleh rasa sedih yang tidak berdaya dan "
              "putus asa. \n";
      cout << "Emosi anda sering terasa tidak stabil dan anda memiliki "
              "kekhawatiran yang berlebihan. \n";
      cout << "Tekanan yang berlebihan membuat kehidupan anda terasa tidak "
              "berharga. \n";
      cout << "Cobalah untuk merasa lebih percaya diri pada diri anda. \n";
      cout << "Yakinlah bahwa anda termasuk orang yang kuat dan pantas untuk "
              "hidup bahagia. \n";
    }

    cout << "Apa anda ingin mengulang program?" << endl;
    cout << "Pilihan anda (ya / tidak) : ";
    cin >> pilihan;

  } while (pilihan == "Ya" || pilihan == "ya" || pilihan == "Yes" ||
           pilihan == "yes");

  cout << "Terima kasih atas partisipasi anda" << endl;
  return 0;
}
