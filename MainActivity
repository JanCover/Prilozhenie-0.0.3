import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.EditText;
import android.widget.TextView;

public class MainActivity extends AppCompatActivity {

    String status = "dor_close";
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }

    public void Send(View view) {
        EditText editText = (EditText)findViewById(R.id.editTextInfo);
        String dor = editText.getText().toString();
        if ("dor_close".equals(status) && "1".equals(dor)) {
            status = "dor_open";
            TextView infoTextView = (TextView)findViewById(R.id.textViewInfo);
            infoTextView.setText(status);
        }
        if ("dor_open".equals(status) && "0".equals(dor)) {
            status = "dor_close";
            TextView infoTextView = (TextView)findViewById(R.id.textViewInfo);
            infoTextView.setText(status);
        }
    }
}
