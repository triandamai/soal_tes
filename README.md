### Hai, Selamat datang👋

Selesaikan Studi Kasus Berikut

1.Implementasikan interface `onTemperatureState` ke `class` CekSuhu

```java
  /**
    *
    * @author Kaila Indonesia
    */
    public interface onTemperatureState {
        void onChange();
        void onDestroy();
    }

```

2. Apa Output Program Dibawah dan berikan penjelasan Algoritmanya

```java
    /**
    *
    * @author Kaila Indonesia
    */
    public class Warna {
        protected String output ="Hijau";
        protected String exceptColor = "Kuning";
        protected List<String> mWarnaList = new ArrayList<>();

        public Warna(List<String> Listwarna){
            this.mWarnaList = Listwarna;
        }
        public String render(){
            for(int i =0;i < mWarnaList.size();i++){
                if(!mWarnaList.get(i).equals(exceptColor)){
                    output += ",";
                    output += mWarnaList.get(i);
                }
            }
            return output;
        }
    }

    public static void main(String[] args) {

        List<String> stringList = new ArrayList<>();
        stringList.add("Merah");
        stringList.add("Hijau");
        stringList.add("Kuning-Kuning");
        stringList.add("Hitam");

        Warna warna = new Warna(stringList);
        System.err.println(warna.render());
    }
```

3. Buatlah sebuah program untuk menghitung gaji karyawan dengan ketentuan sebagai berikut:

Daftar gaji karyawan /bulan

| GOLONGAN |  GAJI POKOK  |  TUNJANGAN |
| -------: | :----------: | ---------: |
|        1 | Rp 1.200.000 | Rp 150.000 |
|        2 | Rp 1.600.000 | Rp 300.000 |
|        3 | Rp 2.350.000 | Rp 350.000 |

Ketentuan:

- Setiap karyawan mendapatkan tunjangan apabila memiliki anak dan sudah menikah
- Tunjangan didapatkan dari tabel diatas dikalikan dengan jumlah anak
- Maksimal jumlah anak yang mendapatkan tunjangan 2 orang anak
- Program tidak harus sama dengan contoh

Contoh Input:

```
====== PERHITUNGAN GAJI KARYAWAN ======


Masukkan Nama Pegawai = ....
Masukkan Golongan = ....
Apakah Sudah Menikah ? (Y,N) = ....
Jumlah Anak ? (1,2,3... dst) = ....




```

Selamat mengerjakan 💡
