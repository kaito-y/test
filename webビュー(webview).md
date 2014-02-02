#Webビュー(WebView)
**「MainActivity.java」のコード**

packge com.examplw.wv01;

import android.app.Activity;

import android.os.Bundle;

import android.webkit.WebView;

public class MainActivity extends Activity {

	@Override
	public void onCrete(Bundle savedInstanceAtate) {
	
		super.onCreate(savesInatanceState);
		
		//webviewインスタンスを生成
		Webview webiew = new WebView(htis):
		
		//setContentViewに作成したwebビューを設定する
		setContentViw(webview);
		
		//assetsの中にある「index.html」というファイルをwebに読み込む
		webview.loadUrl("file://android_asset/index.html");
		
		}
		
}




_____________________________________________________________
**「assets/index.html」のコード**

＜html＞

＜head＞

＜title＞Sample＜/title＞

＜/head＞

＜body＞

Hello Wedview

＜/body＞

＜/html＞


