# -Android-
在Android开发中我们经常会用到日志输入调试程序，通常我们可以借助工具在上线的时候讲日志清除，但是我们可能多个版本迭代，上次的日志可能还有用，这是就不能用清除的方式处理，可以通过表示位来管理日志是否打印
具体用法：在Application启动时初始化
@Override
    public void onCreate() {
    	// TODO Auto-generated method stub
    	super.onCreate();
    	//开启调试日志模式，上线时设置为false即可关闭日志，默认不打印日志
    	DebugLogUtil.getInstance().setDebug(true);
    	//设置输入日志的Tag，默认Tag="Application"
    	DebugLogUtil.getInstance().setFilter("Debug");
    }
