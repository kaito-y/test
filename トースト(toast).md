#トースト(Toast)
package android.sample;

import android.app.Activity;

import android.os.Bundle;

**import android.widget.Toast;**

public class HelloAndroid extends Activity {

    /** Called when the activity is first created. */
    @Override
    public void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.main);
        //トーストの表示
        Toast.makeText(this, "テキスト", Toast.LENGTH_LONG).show();
    }
}