# -Android-DebugLogUtil
具体用法：在Application启动时初始化
DebugLogUtil.getInstance().setDebug(true);//开启调试日志模式，上线时设置为false即可关闭日志，默认不打印日志
DebugLogUtil.getInstance().setFilter("Debug");//设置输入日志的Tag，默认Tag="Application"

