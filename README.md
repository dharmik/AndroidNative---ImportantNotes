AndroidNative---ImportantNotes
==============================

Some ImportantNotes

1) Remove Actionbar in default project :) 

   You need to Apply this property in Androidmanifeast.xml

~~~
<android:theme="@android:style/Theme.NoTitleBar">
~~~

2) Get the name of any image or any video . 

  With the help of this function we can get the name of video or any image


~~~~
public String getFileNameFromUrl(String path) {
		String[] pathArray = path.split("/");
		return pathArray[pathArray.length - 1];
	}
~~~~

3) How to set Bitmap in imageView

  YOu can set that BitMap in ImageView like follow this step
  
  ~~~
  BitmapDrawable ob = new BitmapDrawable(bitmap); // bitmap = Image in Bitmap format
  
  imageView.setBackgroundDrawable(ob);
  ~~~
