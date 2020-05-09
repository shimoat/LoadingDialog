# LoadingDialog
Android 加载框 </br>
# 效果图
<div align=center><img src="https://github.com/shimoat/LoadingDialog/blob/master/image/preview.png"/></div>


使用说明
--
1、项目下的build.gradle添加

```
allprojects {
	repositories {
		...
		maven { url 'https://www.jitpack.io' }
	}
}
```
2、模块下的build.gradle添加依赖

```
dependencies {
    implementation 'com.github.shimoat:LoadingDialog:1.0.0'
}
```
3、在代码中使用

```
private Dialog mLoadingDialog;

public void showLoading() {
    mLoadingDialog = LoadingDialog.createLoadingDialog(this, "加载中...");
}
    
public void hideLoading() {
    LoadingDialog.closeDialog(mLoadingDialog);
}
```