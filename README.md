# tugas-modul-rpl-xr3
## perkenalan
### activity_main.xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:paddingBottom="@dimen/vp"
    android:paddingTop="@dimen/vp"
    android:paddingRight="@dimen/hp"
    android:paddingLeft="@dimen/hp"
    android:orientation="vertical">

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="@string/nama" />

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:textSize="20dp"
        android:layout_marginBottom="20dp"
        android:text="@string/rakha_galih_nugraha_sukma" />

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="@string/ttl" />

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:textSize="20dp"
        android:layout_marginBottom="20dp"
        android:text="@string/ta19" />

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="@string/almt" />

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:textSize="20sp"
        android:layout_marginBottom="20dp"
        android:text="@string/perum" />

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="@string/hp" />

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:textSize="20sp"
        android:layout_marginBottom="20dp"
        android:text="@string/no" />

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="@string/hob" />

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:textSize="20sp"
        android:layout_marginBottom="20dp"
        android:text="@string/mm" />

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="@string/wish" />

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:textSize="20sp"
        android:layout_marginBottom="20dp"
        android:text="@string/mko" />

</LinearLayout>
### strings.xml
<resources>
    <string name="app_name">perkenalan</string>
    <string name="Nama">Nama</string>
    <string name="nama">Nama :</string>
    <string name="rakha_galih_nugraha_sukma">Rakha Galih Nugraha Sukma</string>
    <string name="ttl">Tempat tangggal lahir :</string>
    <string name="ta19">Tulungagung, 19 Desember 2003</string>
    <string name="almt">Alamat :</string>
    <string name="perum">Perum, bangau putih. Blok C no 21</string>
    <string name="hp">No HP :</string>
    <string name="no">081336340166</string>
    <string name="hob">Hobi :</string>
    <string name="mm">Mendengarkan musik</string>
    <string name="wish">Keinginan :</string>
    <string name="mko">Membahagiakan kedua orangtua</string>
</resources>
### dimens.xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <dimen name="vp">16dp</dimen>
    <dimen name="hp">16dp</dimen>
</resources>


## modul 8 (Latihan activity)
### main_activity.xml
<?xml version="1.0" encoding="utf-8"?>
    <LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:paddingBottom="@dimen/activity_vertical_margin"
    android:paddingTop="@dimen/activity_vertical_margin"
    android:paddingRight="@dimen/activity_horizontal_margin"
    android:paddingLeft="@dimen/activity_horizontal_margin"
    android:orientation="vertical">

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="@string/length" />

    <EditText
        android:id="@+id/edt_length"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:inputType="numberDecimal"
        android:lines="1" />

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="@string/width" />

    <EditText
        android:id="@+id/edt_width"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:inputType="numberDecimal"
        android:lines="1" />

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="@string/height" />

    <EditText
        android:id="@+id/edt_height"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:inputType="numberDecimal"
        android:lines="1" />

    <Button
        android:id="@+id/btn_calculate"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="@string/calculate" />

    <TextView
        android:id="@+id/tv_result"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:gravity="center"
        android:text="@string/result"
        android:textSize="24sp"
        android:textStyle="bold" />
    </LinearLayout>
   
### dimens.xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <dimen name = "activity_horizontal_margin">16dp</dimen>
    <dimen name = "activity_vertical_margin">8dp</dimen>
</resources>
    
### strings.xml
<resources>
    <string name="app_name">Produktif Balok</string>
    <string name="width">Lebar</string>
    <string name="height">Tinggi</string>
    <string name="length">Panjang</string>
    <string name="calculate">Hitung</string>
    <string name="result">Hasil</string>
</resources>
    
### MainActivity.java
package com.example.produktifbalok;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.text.TextUtils;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.TextView;

public class MainActivity extends AppCompatActivity implements View.OnClickListener {
    private EditText edtWidth;
    private EditText edtHeight;
    private EditText edtLength;
    private Button btnCalculate;
    private TextView tvResult;
    private static final  String STATE_RESULT = "state_result";
    @Override
    protected void onSaveInstanceState(Bundle outState) {
        super.onSaveInstanceState(outState);
        outState.putString(STATE_RESULT, tvResult.getText().toString());
    }
    @Override
    protected void onCreate(Bundle savedInstanceState){
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

       edtWidth = findViewById(R.id.edt_width);
       edtHeight = findViewById(R.id.edt_height);
       edtLength = findViewById(R.id.edt_length);
       tvResult = findViewById(R.id.tv_result);
       btnCalculate = findViewById(R.id.btn_calculate);
       btnCalculate.setOnClickListener(this);

        if (savedInstanceState != null) {
            String result = savedInstanceState.getString(STATE_RESULT);
            tvResult.setText(result);
        }
    }

    @Override
    public void onClick(View v) {
        if (v.getId() == R.id.btn_calculate){
            String inputLength = edtLength.getText().toString().trim();
            String inputWidth = edtWidth.getText().toString().trim();
            String inputHeight = edtHeight.getText().toString().trim();

            boolean isEmptyFields = false;
            boolean isInvalidDouble = false;

            if (TextUtils.isEmpty(inputLength)){
                isEmptyFields = true;
                edtLength.setError("Field ini tidak boleh kosong");
            }
            if (TextUtils.isEmpty(inputWidth)){
                isEmptyFields = true;
                edtWidth.setError("Field ini tidak boleh kosong");
            }
            if (TextUtils.isEmpty(inputHeight)){
                isEmptyFields = true;
                edtHeight.setError("Field ini tidak boleh kosong");
            }

            Double length = toDouble(inputLength);
            Double width = toDouble(inputWidth);
            Double height = toDouble(inputHeight);

            if (length == null) {
                isInvalidDouble = true;
                edtLength.setError("Field ini harus berupa nomer yang valid");
            }
            if (length == null) {
                isInvalidDouble = true;
                edtLength.setError("Field ini harus berupa nomer yang valid");
            }
            if (length == null) {
                isInvalidDouble = true;
                edtLength.setError("Field ini harus berupa nomer yang valid");
            }
            if (!isEmptyFields && !isInvalidDouble) {
                double volume = length * width * height;
                tvResult.setText(String.valueOf(volume));
            }
            }
    }

    private Double toDouble(String str) {
        try {
            return Double.valueOf(str);
        } catch (NumberFormatException f){
            return null;
        }
    }
}
