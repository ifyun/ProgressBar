# ProgressBar
### Contains CircleProgressBar and ProgressButton.

Cirlce ProgressBar|Progress Button|
------------------|---------------|
![Circle ProgressBar](https://github.com/imcloudfloating/Images/blob/master/circle_progress_bar.gif?raw=true)|![Progress Button](https://github.com/imcloudfloating/Images/blob/master/progress_button.gif?raw=true)

## Gradle:
Add it in your root build.gradle at the end of repositories:
```gradle
	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```
Add the dependency
```gradle
	dependencies {
	        implementation 'com.github.imcloudfloating:ProgressBar:1.1'
	}
```

## Use Cirlce ProgressBar:
```xml
	<com.cloud.progressbar.CircleProgressBar
    	    android:id="@+id/circle_progress"
    	    android:layout_width="180dp"
    	    android:layout_height="180dp"
    	    android:gravity="center"
    	    android:textColor="#80cc33"
    	    android:textSize="22sp"
    	    android:text="Circle ProgressBar"
    	    app:progressBackColor=""#e0e0e0"
    	    app:progressColor="#80cc33"
    	    app:progressWidth="16dp" />
```
If you want a fanshaped progress bar, let progressWidth >= min(layout_width, layout_height)
```java
	cirlceProgressBar.setMinProgress(-100)   //minProgress can be negative, default is 0
    	circleProgressBar.setMaxProgress(100)    //default value is 100
    	circleProgressBar.setProgress(20)
```

## Use Progress Button:
```xml
	<com.cloud.customviews.ProgressButton
    	    android:id="@+id/progress_button"
    	    android:layout_width="240dp"
    	    android:layout_height="wrap_content"
    	    android:textColor="#ffffff"
    	    android:text="Progress Button"
    	    app:cornerRadius="8dp"
    	    app:progressMargin="2dp"
    	    app:progressBackColor="#e0e0e0"
    	    app:progressColor="#80cc33"
    	    app:buttonColor="#80cc33" />
```
```java
	cirlceProgressBar.setMinProgress(-100)   //minProgress can be negative, default is 0
	circleProgressBar.setMaxProgress(100)    //default value is 100
	circleProgressBar.setProgress(20)
```
