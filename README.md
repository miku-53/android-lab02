# Android 实验三：巡检页面整理与 OkHttp 网络请求

## 运行方法
使用 Android Studio 打开项目，同步 Gradle 后，运行到模拟器或真机。
点击页面上的“请求 A203”或“请求 A204”按钮即可发起网络请求并查看回显。

## 三个源码文件职责
1. `MainActivity.kt`：系统入口，负责设置 Compose 内容，安排请求与结果更新。
2. `InspectionScreen.kt`：显示巡检数据、按钮与回调，并计算未检查数量。
3. `InspectionNetwork.kt`：创建 OkHttpClient，执行网络请求，处理响应和异常。