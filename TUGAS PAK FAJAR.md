
```dart
void main() {

  // Aritmatika: Operasi matematika dasar

  int hitungNilai(int matematika, int sains, int bahasaInggris) {

    return (matematika + sains + bahasaInggris) ~/ 3; // menggunakan ~/ untuk pembagian integer

  }

  

  // List, Set, Map (Dictionary), dan Symbol

  List<int> nilai = [80, 70, 90];

  Set<String> mataPelajaranUnik = {"Matematika", "Sains", "Bahasa Inggris"};

  Map<String, dynamic> siswa = {"nama": "John", "umur": 20};

  

  // Percabangan: Penggunaan pernyataan if-else

  int rataRata = hitungNilai(nilai[0], nilai[1], nilai[2]);

  if (rataRata >= 90) {

    print("Kamu mendapat A!");

  } else if (rataRata >= 80) {

    print("Kamu mendapat B!");

  } else {

    print("Kamu mendapat C!");

  }

  

  // Perulangan: Penggunaan loop seperti for dan while

  for (String pelajaran in mataPelajaranUnik) {

    print("Mata Pelajaran: $pelajaran");

  }

  

  int i = 0;

  while (i < nilai.length) {

    print("Nilai: ${nilai[i]}");

    i++;

  }

  

  // Function: Definisi dan penggunaan fungsi

  void cetakInfoSiswa(Map<String, dynamic> siswa) {

    print("Nama: ${siswa["nama"]}");

    print("Umur: ${siswa["umur"]}");

  }

  

  cetakInfoSiswa(siswa);

  

  // Scope: Pengertian ruang lingkup variabel dalam program

  int x = 10;

  

  void fungsiDalam() {

    int y = 20;

    print("Fungsi dalam: $y");

  }

  

  fungsiDalam();

  print("Fungsi luar: $x");

  

  // Closure/Recursive Function: Penggunaan fungsi rekursif dan penutupan (closure)

  int faktorial(int n) {

    if (n == 0) {

      return 1;

    } else {

      return n * faktorial(n - 1);

    }

  }

  

  print("Faktorial dari 5: ${faktorial(5)}");

}
```