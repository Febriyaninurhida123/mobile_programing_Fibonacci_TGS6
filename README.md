```
Febriyani NUrhida
312210222
TI.22.A2
````
# Fibonacci Sequence
Fibonacci Sequence (Deret angka Fibonacci) adalah deret angka yang diperoleh dengan menjumlahkan dua angka didepannya / sebelumnya:

1, 1, 2, ...
1 + 2 = 3 ( 1, 1, 2, 3, ... )
2 + 3 = 5 ( 1, 1, 2, 3, 5, ... )
3 + 5 = 8 ( 1, 1, 2, 3, 5, 8, ... )

## Langkah Praktikum
![9335406bb80512c](https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/78847147-815c-4974-85bb-acbd1dc7213a)

1. Dalam folder app > res > layout di panel Project > Android , klik dua kali file Activity_main.xml untuk membukanya, jika belum dibuka.
2. Klik tab Desain jika belum dipilih. Anda menggunakan tab Desain untuk memanipulasi elemen dan tata letak, dan tab Kode untuk mengedit kode XML untuk tata letak. Tab Split memperlihatkan kode dan desain XML.
3. Panel Palet memperlihatkan elemen UI yang dapat Anda gunakan dalam tata letak aplikasi Anda.
4. Panel pohon komponen memperlihatkan hierarki tampilan elemen UI. Viewelemen diorganisasikan ke dalam hierarki pohon orang tua dan anak, di mana seorang anak mewarisi atribut dari induknya. Pada gambar di atas, TextViewadalah turunan dari ConstraintLayout . Anda akan mempelajari elemen-elemen ini nanti dalam pelajaran ini.
5. Panel desain dan cetak biru editor tata letak menampilkan elemen UI dalam tata letak. Pada gambar di atas, tata letak hanya memperlihatkan satu elemen: a TextViewyang menampilkan "Hello World".
6. Tab Atribut menampilkan panel Atribut untuk mengatur properti elemen UI.
7. Ikuti langkah-langkah berikut untuk menambahkan Button:
![25c3a2ee7e419b4a](https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/332eb1ce-03aa-4437-b83d-7c1e9ec5f389)
- Mulailah dengan awal yang bersih. Elemen tersebut TextViewtidak diperlukan, jadi selagi masih dipilih, tekan tombol Delete atau pilih Edit > Delete . Anda sekarang memiliki tata letak yang benar-benar kosong.
- Seret Tombol dari panel Palet ke posisi mana pun di tata letak. Jika Anda melepaskannya Buttondi area tengah atas tata letak, batasan akan muncul secara otomatis. Jika tidak, Anda dapat menyeret batasan ke atas, samping kiri, dan kanan tata letak seperti yang ditunjukkan pada gambar animasi di bawah.
- Seret Tombol lain dari panel Palet ke tengah tata letak seperti yang ditunjukkan pada gambar animasi di bawah. Sambung otomatis mungkin memberikan batasan horizontal untuk Anda (jika tidak, Anda dapat menyeretnya sendiri).
- Seret batasan vertikal ke bagian bawah tata letak (lihat gambar di bawah).
![93d4cd13795d4b2f](https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/195ea7d3-79aa-4b06-a991-3f4479329f58)

![f089d8dd87c70a5d](https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/4e9c7e27-da70-4b2c-bb4c-c6547f016b17)

- Kontrol ketinggian . Kontrol ini menentukan layout_heightatribut dan muncul dalam dua segmen di sisi atas dan bawah kotak. Sudutnya menunjukkan bahwa kontrol ini disetel ke wrap_content, yang berarti kontrol Viewakan melebar secara vertikal sesuai kebutuhan agar sesuai dengan isinya. Angka "0" menunjukkan margin standar yang disetel ke 0dp.
- Kontrol lebar . Kontrol ini menentukan layout_widthdan muncul dalam dua segmen di sisi kiri dan kanan kotak. Sudutnya menunjukkan bahwa kontrol ini disetel ke wrap_content, yang berarti kontrol Viewakan melebar secara horizontal sesuai kebutuhan agar sesuai dengan kontennya, hingga margin 0dp.
Tombol tutup panel atribut . Klik untuk menutup panel.
kuti langkah ini:
![d6e227589ef958a8](https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/fa065731-12ae-424a-835f-cb58bc24291a)

* Pilih bagian atas Buttondi panel Component Tree .
* Klik tab Atribut di sisi kanan jendela editor tata letak.
* Atur margin kiri, kanan, dan atas menjadi 8dp (jika belum disetel)
Klik kontrol lebar dua kali—klik pertama mengubahnya menjadi Tetap dengan garis lurus, dan klik kedua mengubahnya menjadi Cocokkan Batasan dengan kumparan pegas, seperti yang ditunjukkan pada gambar animasi di bawah.
![ca13854a3378781c](https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/675e7d3c-ee6b-4fef-a82c-a7ad6425d2c0)
Sebagai hasil dari perubahan kontrol lebar, layout_widthatribut di panel Atribut memperlihatkan nilai match_constraintdan Buttonelemen membentang secara horizontal untuk mengisi ruang antara sisi kiri dan kanan tata letak.
* Pilih yang kedua Button, dan buat perubahan yang sama seperti layout_widthpada langkah sebelumnya, seperti yang ditunjukkan pada gambar di bawah.
  ![4ccb5308188a077c](https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/fa6f9ff4-b1a9-497b-b1fd-137b1da000e2)
8. Untuk mengidentifikasi masing-masing Viewsecara unik dalam Activitytata letak, setiap Viewatau Viewsubkelas (seperti Button) memerlukan ID unik. Dan agar dapat berguna, Buttonelemen tersebut memerlukan teks. Viewelemen juga dapat memiliki latar belakang yang dapat berupa warna atau gambar.

Panel Atribut menawarkan akses ke semua atribut yang dapat Anda tetapkan ke sebuah Viewelemen. Anda dapat memasukkan nilai untuk setiap atribut, misalnya atribut android:id, background, textColor, dan text.

Gambar animasi berikut menunjukkan cara melakukan langkah-langkah ini:

- Setelah memilih yang pertama Button, edit bidang ID di bagian atas panel Atribut menjadi button_toast untuk android:idatribut, yang digunakan untuk mengidentifikasi elemen dalam tata letak.
- Setel backgroundatribut ke @color/colorPrimary . (Saat Anda memasukkan @c , pilihan muncul untuk memudahkan pemilihan.)
- Setel textColoratribut ke @android:color/white .
- Edit textatribut ke Toast .
![3b450a71f7046f9b](https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/7fad6a72-7d5a-4642-837d-8a3b6dba2274)
- Lakukan perubahan atribut yang sama untuk yang kedua Button, menggunakan button_count sebagai ID, Count untuk textatribut, dan warna yang sama untuk latar belakang dan teks seperti langkah sebelumnya.
9. Tambahkan TextView dan batasannya
Seperti yang diperlihatkan dalam gambar animasi di bawah, seret a TextViewdari panel Palet ke bagian atas tata letak, dan seret batasan dari atas TextViewke pegangan di bagian bawah ToastButton . Ini membatasi TextViewberada di bawah Button.
![4e57585c07b24314](https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/9a3eda7d-8937-4224-ac8b-efcb61f54704)
- Seperti yang diperlihatkan dalam gambar animasi di bawah, seret batasan dari bagian bawah ke TextViewpegangan di bagian atas Count ,Button dan dari sisi TextViewke sisi tata letak. Hal ini membatasi untuk TextViewberada di tengah-tengah tata letak antara dua Buttonelemen.
![63ad84d10cc1e9df](https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/7b542af3-d3a9-453b-8329-a16707e08312)
- ubah text nya jadi 0.
10. Buka kode XML untuk tata letak
  di sini saya sudah membuat kodenya :
  ```xml
  <?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="10dp"
    tools:context=".ThirdActivity">

    <Button
        android:id="@+id/button_toast"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginTop="8dp"
        android:layout_marginEnd="8dp"
        android:background="@color/colorPrimery"
        android:text="@string/button_label_toast"
        android:textColor="@android:color/white"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        android:onClick="showToast" />


    <Button
        android:id="@+id/button_count"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="8dp"
        android:background="@color/colorPrimery"
        android:text="Button"
        android:textColor="@android:color/white"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        android:onClick="countUp" />
    <TextView
        android:id="@+id/show_count"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="8dp"
        android:background="#FFFF00"
        android:gravity="center_vertical"
        android:text="0"
        android:textAlignment="center"
        android:textColor="@color/colorPrimery"
        android:textSize="160sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toTopOf="@+id/button_count"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button_toast" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
<img width="1080" alt="Cuplikan layar 2023-11-01 213021" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/aad20b30-dc82-41a9-ad31-67dc699c467d">


design nya akan tampak seperti ini :
<img width="1080" alt="Cuplikan layar 2023-11-01 212559" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/5ee07361-7c4d-4d2f-a771-ae426926ed74">
10. Edit pengendali Tombol Hitung
sekarang akan mengedit countUp()metodenya— pengendali klik HitungButton di MainActivity- sehingga menampilkan hitungan saat ini setelah Hitungan disadap. Setiap ketukan menambah hitungan satu per satu.

Kode untuk handler harus:
- Pantau hitungannya seiring perubahannya.
- Kirim hitungan yang diperbarui ke untuk TextViewmenampilkannya.

di sini saya sudah membuat activity baru bernama Third_Activity dan mengkodenya

```java
package com.example.fibonacci;

import android.os.Bundle;
import android.view.View;
import android.widget.TextView;
import android.widget.Toast;

import androidx.appcompat.app.AppCompatActivity;

public class ThirdActivity extends AppCompatActivity {
    int first = 0;
    int second = 1;
    TextView Fibonacci;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_fibonacci);

        Fibonacci = findViewById(R.id.show_count);
        updateFibonacciText();
    }

    public void showToast(View view) {
        Toast.makeText(this, "Fibonacci", Toast.LENGTH_SHORT).show();
    }

    public void countUp(View view) {
        int next = first + second;
        first = second;
        second = next;
        updateFibonacciText();
    }

    private void updateFibonacciText() {
        Fibonacci.setText(Integer.toString(second));
    }
}
```
<img width="1080" alt="Cuplikan layar 2023-11-01 212957" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/873262b3-5e14-4463-a986-71056e83e91f">
11. Jalankan aplikasi untuk memverifikasi bahwa hitungan bertambah ketika Anda mengetuk tombol Hitung .
<img width="1080" alt="Cuplikan layar 2023-11-01 213614" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/532b6e27-b403-453b-b43f-3835060972c2">

- saat di klik lagi tombol count akan muncul angka 1, 2, 3, 5, dst:
<img width="1080" alt="Cuplikan layar 2023-11-01 213614" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/d25ce1c5-bd31-49dd-8f6e-c18e1eb06c5c">
<img width="1080" alt="Cuplikan layar 2023-11-01 213633" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/7513f1a0-ba55-40e6-a8e3-7a62776daffa">
<img width="1080" alt="Cuplikan layar 2023-11-01 213648" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/4a379670-a0a9-4eab-88db-28cc024736f6">
<img width="1080" alt="Cuplikan layar 2023-11-01 213707" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/76d0ab92-70b5-4514-9a88-5d6eeb112746">
- saat di klik button Toast akan muncul tulisan fibonacci :
  <img width="1080" alt="Cuplikan layar 2023-11-01 213732" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/62e1d36d-8789-4673-9027-3938d657bad3">

## Selanjutnya adalah membuat button dan text view baru meliputi:
* button restart(back),
* button max
* textview untuk input nilai maximalnya
## Layout
Pada layout ini, saya membuat tiga button dan satu textview :
1. `button_limit`, berfungsi sebagai tombol “Set Limit” yang nantinya ketika di tekan akan muncul sebuah pop-up untuk masukan limit angka yang ingin kita hitung.
2. `button_count`, berfungsi sebagai tombol “count” yang nantinya ketika tombol ditekan akan menghitung bilangan fibonaccinya sesuai dengan yang kita limit. Juga berbeda warna pada setiap angka, agar tidak keliru.
3. 'button_restart', berfungsi sebagai tombol restart yang nantinya angka akan kembali ke awal.
4. Textview `show_count`, yang berfungsi untuk menampilkan angka atau bilangan fibonaccinya yang tepat berada di tengah.
```xml
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:ignore="ExtraText"
    tools:context="com.example.fibonacci.ThirdActivity">


    <Button
        android:id="@+id/button_limit"
        android:layout_width="409dp"
        android:layout_height="84dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="16dp"
        android:layout_marginEnd="8dp"
        android:background="@color/colorPrimary"
        android:onClick="setLimit"
        android:text="Masukkan Angka Limit"
        android:textColor="@android:color/white"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.507"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        tools:ignore="UsingOnClickInXml,VisualLintButtonSize" />

    <Button
        android:id="@+id/button_count"
        android:layout_width="190dp"
        android:layout_height="80dp"
        android:layout_marginStart="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="8dp"
        android:background="@color/colorPrimary"
        android:onClick="countUp"
        android:text="Count"
        android:textColor="@android:color/white"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        tools:ignore="UsingOnClickInXml,VisualLintButtonSize" />

    <Button
        android:id="@+id/button_restart"
        android:layout_width="190dp"
        android:layout_height="80dp"
        android:layout_marginStart="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="8dp"
        android:background="@color/colorPrimary"
        android:onClick="back1"
        android:text="Restart"
        android:textColor="@android:color/white"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="1.0"
        app:layout_constraintStart_toStartOf="parent"
        tools:ignore="UsingOnClickInXml" />

    <TextView
        android:id="@+id/show_count"
        android:layout_width="417dp"
        android:layout_height="649dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="8dp"
        android:background="#FFFF00"
        android:gravity="center_vertical"
        android:text="0"
        android:textAlignment="center"
        android:textColor="@color/colorPrimary"
        android:textSize="160sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toTopOf="@id/button_count"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@id/button_limit"
        app:layout_constraintVertical_bias="0.0"
        tools:ignore="RtlCompat" />
```
<img width="1080" alt="Cuplikan layar 2023-11-02 110621" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/2598e85d-081f-4595-a409-0b0cdb2f7649">

designnya akan seperti ini :
<img width="1080" alt="Cuplikan layar 2023-11-02 111111" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/68bd6e93-f338-4e0f-a4c0-8b92b60f799b">

## Java class
Pada Java class `MainActivity.java` berisi semua coding untuk menjalankan aplikasi. Seperti fungsi untuk tombol-tombol, dialog set limit, warna yang berbeda pada setiap angka, lalu warna background yang bisa berubah dan rumus bilangan fibonacci.
</androidx.constraintlayout.widget.ConstraintLayout>
Berikut adalah coding pada menu layout :
```java
package com.example.fibonacci;

import android.app.AlertDialog;
import android.content.DialogInterface;
import android.graphics.Color;
import android.os.Bundle;
import android.view.View;
import android.widget.EditText;
import android.widget.TextView;
import androidx.appcompat.app.AppCompatActivity;


public class ThirdActivity extends AppCompatActivity {
    private TextView show_count;
    private int count = 1;
    private long fibNMinus1 = 1;
    private long fibNMinus2 = 1;
    private int limit = -1; // Inisialisasi limit dengan nilai default

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_fibonacci);

        show_count = findViewById(R.id.show_count);
    }

    public void countUp(View view) {
        if (count == 1) {
            show_count.setText("0");
        }

        else {
            if (limit != -1 && count > limit) {
                // Jika count melebihi limit, atur ulang perhitungan
                count = 1;
                fibNMinus1 = 1;
                fibNMinus2 = 0;
                show_count.setText(getString(R.string.count_initial_value));
            }
            else {
                long fibCurrent = fibNMinus1 + fibNMinus2;
                fibNMinus2 = fibNMinus1;
                fibNMinus1 = fibCurrent;

                //Mengatur warna teks berdasarkan angka Fibonacci
                int colorResId = R.color.orange; // Warna Default
                switch (count % 11) {
                    case 1:
                        colorResId = R.color.orange; // Warna Orange
                        break;
                    case 2:
                        colorResId = R.color.hijaumuda; // Warna Hijau Muda
                        break;
                    case 3:
                        colorResId = R.color.purple; // Warna Ungu
                        break;
                    case 4:
                        colorResId = R.color.salem; // Warna Salem
                        break;
                    case 5:
                        colorResId = R.color.birumuda; // Warna Biru Muda
                        break;
                    case 6 :
                        colorResId = R.color.purple; // Warna Kuning
                        break;
                    case 7:
                        colorResId = R.color.hijau; // Warna Hijau
                        break;
                    case 8:
                        colorResId = R.color.cream; // Warna Cream
                        break;
                    case 9:
                        colorResId = R.color.pink; // Warna Pink
                        break;
                    case 10:
                        colorResId = R.color.biru; // Warna Biru
                        break;
                    case 11:
                        colorResId = R.color.colorAccent; // Warna Pink Tua
                        break;
                }
                show_count.setTextColor(getResources().getColor(colorResId));
                show_count.setText(String.valueOf(fibCurrent));
                show_count.setBackgroundColor(Color.YELLOW);
            }
        }

        count++;
    }

    public void back1(View view) {
        count = 1;
        fibNMinus1 = 1;
        fibNMinus2 = 0;
        show_count.setText("0"); // Mengatur teks pada TextView menjadi "0"
        show_count.setTextColor(getResources().getColor(R.color.colorPrimary)); // Mengatur warna teks kembali ke warna default
        show_count.setBackgroundColor(Color.YELLOW); // Menghapus latar belakang yang mungkin telah diatur sebelumnya
    }


    public void setLimit(View view) {
        // Create and display a dialog to set the limit
        AlertDialog.Builder builder = new AlertDialog.Builder(this);
        builder.setTitle("Set Limit");

        final EditText input = new EditText(this);
        input.setInputType(android.text.InputType.TYPE_CLASS_NUMBER);
        builder.setView(input);

        builder.setPositiveButton("OK", new DialogInterface.OnClickListener() {
            @Override
            public void onClick(DialogInterface dialog, int which) {
                // Get the limit from the input and set it for calculations
                String limitStr = input.getText().toString();
                limit = Integer.parseInt(limitStr);
            }
        });

        builder.setNegativeButton("Cancel", new DialogInterface.OnClickListener() {
            @Override
            public void onClick(DialogInterface dialog, int which) {
                dialog.cancel();
            }
        });

        builder.show();
    }
}
```
<img width="1080" alt="Cuplikan layar 2023-11-02 110734" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/2151c47a-0ffc-41cd-90d1-7f823c6a6b06">

#### hasilnya saat di run :

<img width="1080" alt="Cuplikan layar 2023-11-02 111353" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/50654100-d09b-4ff0-af69-586b83639319">

#### saat diklik button limit akan muncul :
<img width="1080" alt="Cuplikan layar 2023-11-02 111548" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/778cc9ed-f887-42a0-8d69-8d8b6fb94de4">

#### setelah di set maka tinggal klik count hingga mencapai batas maksimum:
<img width="1080" alt="Cuplikan layar 2023-11-02 111353" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/f2d7ab4d-f244-4c29-83ff-1f8a29c1947c">
<img width="1080" alt="Cuplikan layar 2023-11-02 111611" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/44a309d5-1655-40bc-a1cb-f0b228e64100">
<img width="1080" alt="Cuplikan layar 2023-11-02 111628" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/9d1534cc-bb8b-4ef6-9e10-e77ff0959f44">
<img width="1080" alt="Cuplikan layar 2023-11-02 111650" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/7e22c82d-381e-45c7-9afe-b2257b268933">
<img width="1080" alt="Cuplikan layar 2023-11-02 111711" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/2aa01ff9-29a1-4b23-a89e-9cec6656430c">

#### saat di klik restart maka akan kembali ke nol seperti berikut:
<img width="1080" alt="Cuplikan layar 2023-11-02 111739" src="https://github.com/Febriyaninurhida123/mobile_programing_Fibonacci_TGS6/assets/90132092/df9d29ed-5685-424a-9f77-53ae16a438d3">

# sekian dan terima kasih 
