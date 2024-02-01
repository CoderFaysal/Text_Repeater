# Text Repeater

```
public class MainActivity extends AppCompatActivity {

    EditText get_input, get_number;
    Button btn;
    TextView text_output;

    String text ="";

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        get_input = (EditText) findViewById(R.id.get_input);
        text_output = (EditText) findViewById(R.id.text_output);
        get_number = (EditText) findViewById(R.id.get_number);
        btn = (Button) findViewById(R.id.btn);

        btn.setOnClickListener(new.View.OnClickListener()) {
            @Override

            public void onClick(View v){
                String input = get_input.getText().toString();
                int number = Integer.parseInt(get_number.getText().toString());

                for (int i=0; i < number; i++){
                    text = text + input + " ";
                }
                text_output.setText(text);
        }
    });
    }
}
```
