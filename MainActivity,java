package com.example.user.autocomplete;

import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.ArrayAdapter;
import android.widget.AutoCompleteTextView;
import android.widget.Button;
import android.widget.EditText;

import java.util.ArrayList;

public class MainActivity extends AppCompatActivity {

    EditText edtIncluir;
    EditText edtExcluir;
    Button btnIncluir;
    Button btnExcluir;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        edtIncluir = (EditText)findViewById(R.id.edtIncluir);
        edtExcluir = (EditText)findViewById(R.id.edtExcluir);
        btnIncluir = (Button)findViewById(R.id.btnIncluir);
        btnExcluir = (Button)findViewById(R.id.btnExcluir);

        ArrayAdapter<String> adapter = new ArrayAdapter<String>(this, android.R.layout.simple_dropdown_item_1line, lista);
        AutoCompleteTextView textView = (AutoCompleteTextView) findViewById(R.id.minhaLista);
        textView.setAdapter(adapter);

        lista.add("Robson");
        lista.add("Rosemiro");
        lista.add("Rosivaldo");
        lista.add("Rosilauro");
        lista.add("Rosegerson");
        lista.remove("Rosegerson");
    }

    ArrayList<String> lista = new ArrayList<String>();

    public void Incluir(View v){
        String nome = edtIncluir.getText().toString();
        lista.add(nome);
    }

    public void Excluir(View v){
        String nome = edtExcluir.getText().toString();
        lista.remove(nome);
    }
}
