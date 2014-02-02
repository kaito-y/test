#イベント(Event)
package com.example.screen05;

import android.app.Activity;

import android.os.Bundle;

import android.view.Menu;

import android.view.MenuItem;

import android.widget.Toast;

public class MainActivity extends Activity {

	@Override
	protected void onCreate(Bundle savedInstanceState) {
	super.onCreate(savedInstanceState);
		setContentView(R.layout.main);
	 }
	 //メニューボタンが押されたときに実行される
	 @Override
	 public boolean onCreateOptionsMenu(Menu menu) {
	 //メニューを追加
	 menu.add(Menu.NOME,0,Menu.NONE,"Menu1");
	 menu.add(Menu.NOME,1,Menu.NONE,"Menu2");
	 return super.onCreateOptionsMenu(menu);
	}
	 //メニューが選択されたときに実行される
	 @Override
	 public boolean onPtionsItemSeleced(Menu item) {
	 
	 //選択されたIDを確認
	 switch (item,getItemId()) {
	 	case 0:
	 		Tost.makeText(this,"Menu1",Tost.LENGTH_SHORT).
	 		break;
	 	case 1;
		  tost.makeText(this,"Menu2",Toast.LENGTH_SHORT).show();
		  break;
		}
		 return true;
	}
}
	 		