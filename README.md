Barista
=======
TODO (@davidBcn proposals):  
- Remove AT prefix :D I am jelous I don't have DF objects :D
- TfButton --> TypeFaceButton ... I don't really like Tf

**ATPtogressBar01**

usage:<br>
place the progress bar inside your xml layout:<br>
```xml
<com.antoniotari.android.widget.progressbar.ATProgressbar01
    android:id="@+id/at_progressBar"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:layout_alignParentBottom="true"
    android:layout_alignParentLeft="true"
    android:text="@+id/ProgressTextView01" >
</com.antoniotari.android.widget.progressbar.ATProgressbar01>
```
on your Activity or Fragment:<br>
```java
protected ATProgressbar01 pBar;
pBar = (ATProgressbar01)findViewById(R.id.at_progressBar);
pBar.startAnimation();
```
To stop the progress bar
```java
if(pBar!=null){
    pBar.dismiss();
}
```
onDestroy or onDestroyView, to clean the memory:<br>
```java
pBar.clean();
pBar=null;
```
The progress bar can be initialized with any color:<br>
```java
pBar = (ATProgressbar01)rootView.findViewById(R.id.at_progressBar_1);
int[] colors={Color.GRAY,Color.BLUE,Color.BLACK,Color.CYAN,Color.YELLOW,Color.RED,Color.WHITE,Color.GREEN,Color.MAGENTA};
pBar.setColors(colors);
```
