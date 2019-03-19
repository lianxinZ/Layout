# 实验二 Android布局
## 1. LinearLayout
### 关键代码：
~~~
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#000000"
    android:orientation="vertical"
    tools:context=".MainActivity">

        <LinearLayout
            android:id="@+id/one"
            android:layout_width="match_parent"
            android:layout_height="60dp"
            android:orientation="horizontal">

            <TextView
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="one,one"
                android:textColor="#ffffff" />

            <TextView
                android:layout_width="30dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="one,two"
                android:textColor="#ffffff" />

            <TextView
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="one,three"
                android:textColor="#ffffff" />

            <TextView
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="one,four"
                android:textColor="#ffffff" />
        </LinearLayout>

        <LinearLayout
            android:id="@+id/two"
            android:layout_width="match_parent"
            android:layout_height="60dp"
            android:orientation="horizontal">

            <TextView
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="two,one"
                android:textColor="#ffffff" />

            <TextView
                android:layout_width="30dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="two,two"
                android:textColor="#ffffff" />

            <TextView
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="two,three"
                android:textColor="#ffffff" />

            <TextView
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="two,four"
                android:textColor="#ffffff" />
        </LinearLayout>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="60dp"
            android:orientation="horizontal">

            <TextView
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="three,one"
                android:textColor="#ffffff" />

            <TextView
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="three,two"
                android:textColor="#ffffff" />

            <TextView
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="three,three"
                android:textColor="#ffffff" />

            <TextView
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="three,four"
                android:textColor="#ffffff" />
        </LinearLayout>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="60dp"
            android:orientation="horizontal">

            <TextView
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="four,one"
                android:textColor="#ffffff" />

            <TextView
                android:layout_width="30dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="four,two"
                android:textColor="#ffffff" />

            <TextView
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="four,three"
                android:textColor="#ffffff" />

            <TextView
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:background="@drawable/textview_border"
                android:gravity="center"
                android:text="four,four"
                android:textColor="#ffffff" />
        </LinearLayout>

        <Button
            android:id="@+id/b1"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="center"

            android:text="下一个" />

</LinearLayout>
~~~
### 结果截图：
<image width='250dp' hight='450dp' src="https://github.com/lianxinZ/project2.0/blob/master/images/project2-1.jpg">
  
  ## 2.RelativeLayout
  ### 关键代码：
  ~~~
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".Main2Activity">
    <TextView
        android:id="@+id/t1"
        android:layout_width="80dp"
        android:layout_height="80dp"
        android:background="#ff0000"
        android:text="RED"
        android:gravity="center"
        android:layout_alignParentLeft="true"
        />
    <TextView
        android:id="@+id/t2"
        android:layout_width="80dp"
        android:layout_height="80dp"
        android:background="#ff5500"
        android:text="ORANGE"
        android:gravity="center"
        android:layout_centerHorizontal="true"
        />
    <TextView
        android:id="@+id/t3"
        android:layout_width="80dp"
        android:layout_height="80dp"
        android:background="#ffee00"
        android:text="YELLOW"
        android:gravity="center"
        android:layout_alignParentRight="true"/>
    <TextView
        android:id="@+id/t4"
        android:layout_width="80dp"
        android:layout_height="80dp"
        android:background="#002fff"
        android:text="BLUE"
        android:gravity="center"
        android:layout_below="@id/t3"
        android:layout_centerHorizontal="true"
        android:layout_marginTop="50dp"
        />

    <TextView
        android:id="@+id/t5"
        android:layout_width="80dp"
        android:layout_height="80dp"
        android:background="#aa00ff"
        android:text="INDIGO"
        android:gravity="center"
        android:layout_below="@id/t3"
        android:layout_toRightOf="@id/t4"
        android:layout_marginTop="50dp"
        android:layout_marginLeft="20dp"
        />

    <TextView
        android:id="@+id/t6"
        android:layout_width="80dp"
        android:layout_height="80dp"
        android:background="#00ff04"
        android:text="GREEN"
        android:gravity="center"
        android:layout_marginTop="50dp"
        android:layout_marginRight="20dp"
        android:layout_below="@id/t3"
        android:layout_toLeftOf="@id/t4"/>

    <TextView
        android:id="@+id/t7"
        android:layout_width="match_parent"
        android:layout_height="70dp"
        android:background="#ff77c6"
        android:text="VIOLET"
        android:gravity="center"
        android:layout_marginTop="50dp"
        android:layout_below="@id/t6"/>

    <Button
        android:id="@+id/b2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="下一个"
        android:layout_centerHorizontal="true"
        android:layout_below="@id/t7"/>

</RelativeLayout>

~~~
### 结果截图：
<image width='250dp' hight='450dp' src="https://github.com/lianxinZ/project2.0/blob/master/images/project2-2.jpg">
  
## 3.TableLayout
### 关键代码：
~~~
<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#000000"
    tools:context=".Main3Activity">

    <TableLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:stretchColumns="0">

        <TableRow>
            <TextView
                android:text="Open..."
                android:layout_marginLeft="30dp"
                android:textColor="#FFFFFF"
                />
            <TextView
                android:text="Ctrl-O"
                android:layout_marginRight="30dp"
                android:textColor="#FFFFFF"
                />
        </TableRow>
        <TableRow>
            <TextView
                android:text="Save..."
                android:layout_marginLeft="30dp"
                android:textColor="#FFFFFF"
                />
            <TextView
                android:text="Ctrl-S"
                android:layout_marginRight="30dp"
                android:textColor="#FFFFFF"
                />
        </TableRow>
        <TableRow>
            <TextView
                android:text="Save As..."
                android:textColor="#FFFFFF"
                android:layout_marginLeft="30dp"
                />
            <TextView
                android:text="Ctrl-Shift-S"
                android:textColor="#FFFFFF"
                android:layout_marginRight="30dp"
                />
        </TableRow>
        <View  android:layout_height="5px"
            android:layout_width="match_parent"
            android:background="#ffffff"

            />
        <TableRow>
            <TextView
                android:text="X-Import"
                android:layout_marginLeft="30dp"
                android:textColor="#FFFFFF"
                />

        </TableRow>
        <TableRow>
            <TextView
                android:text="X-Export"
                android:layout_marginLeft="30dp"
                android:textColor="#FFFFFF"
                />
            <TextView
                android:text="Ctrl-E"
                android:layout_marginRight="30dp"
                android:textColor="#FFFFFF"
                />
        </TableRow>
        <View  android:layout_height="5px"
            android:layout_width="match_parent"
            android:background="#ffffff"

            />
        <TableRow>
            <TextView
                android:text="Quit"
                android:layout_marginLeft="30dp"
                android:textColor="#FFFFFF"
                />
        </TableRow>
    </TableLayout>





</android.support.constraint.ConstraintLayout>
~~~
### 结果截图：
<image width='250dp' hight='450dp' src="https://github.com/lianxinZ/project2.0/blob/master/images/project2-3.jpg">
