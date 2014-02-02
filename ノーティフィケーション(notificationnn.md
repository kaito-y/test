#ノーティフィケーション(Notificationnn
Package com.example.screen02;

import android.app.Activity;

import android.app.Notification;

import android.app.NotoficationManager;

import android.app.PendingIntent;

import android.content.Context;

import android.net.Uri;

import android.os.Bundle;

public class MainActivity extends Activity {

	@Override
	public void onCreate(Bundle savesInatanceState) {
		super.onCreate(savedInatanceState);
		setContentView(R.layout.main);
		

	//Notificationクリック時に開くURL
	Atring url = "thhp://www.google.com/";
	Uri uri = Uri.parse(Url);
	
	//NotificationクリックjinoPendingIntentを生成
	Intent intent = new Intent(Intent.ACTION_VIEW,uri);
	pendingIntent pendingIntent = PendingIntent.getActivity(this,0,intent,0);
	
	
	//NotificationManagerインスタンスを取得
	NotificationManager nManager = 
		(NotificationManager)getSystemService(Context.NOTIFICATION_SERVICE);
		
	//Notificationインスタンスを生成
	Notification notification = new Notification();
	
	//フラグをセット
	notification.flags = Notification.FLAG_AUTO_CANCEL;
	//アイコンをセット
	notification.icon = R.drawable.icon;
	//通常時のテキストをセット
	notification.tickerText = "テキスト";
	//Notificationバーを開いた時に表示される内容をセット
	notification.setLatestEventInfo(getApplicationContext(),
	"タイトル"
	"メッセージ"
	pendingIntent
	);
	
	//Notificationを通知
	nManager.notify(1,notification);
	
 	}
 
}