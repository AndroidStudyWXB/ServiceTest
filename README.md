问题：onServiceConnected() 和 onServiceDisconnected()方法未执行，如何知道服务和活动是否绑定成功？
解决：	@Override
		public IBinder onBind(Intent intent) {
		-    return null;
		+    return mBinder;
		}
