AndroidNative---ImportantNotes
==============================

Some ImportantNotes


<b>1) Remove Actionbar in default project :) </b>

   You need to Apply this property in Androidmanifeast.xml

~~~
<android:theme="@android:style/Theme.NoTitleBar">
~~~


<b>2) Get the name of any image or any video . </b>

  With the help of this function we can get the name of video or any image


~~~~
public String getFileNameFromUrl(String path) {
		String[] pathArray = path.split("/");
		return pathArray[pathArray.length - 1];
	}
~~~~


<b>3) How to set Bitmap in imageView</b>

  YOu can set that BitMap in ImageView like follow this step
  
  ~~~
  BitmapDrawable ob = new BitmapDrawable(bitmap); // bitmap = Image in Bitmap format
  
  imageView.setBackgroundDrawable(ob);
  ~~~
  
<b>4) Notify Changes to Adapter in Listview</b>

   With the help of this lines you can send posotion that which Row have you click or which Update 
   Other second line means to like in simple language <b>Refresh</b>
   
   ~~~
   adapter.selectedPosition = position;
   adapter.notifyDataSetChanged();
   ~~~
