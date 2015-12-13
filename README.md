# AndroidLayout

##View
* TextView
* EditText
* Button
* ImageView

##View Group
* LinearLayout
* TableLayout
* RelativeLayout(相対的に指定)
* FrameLayout(重ねて表示)

##LinearLayout
縦に並べる場合  
```
android:orientation="vertical"
```

横に並べる場合  
```
android:orientation="horizontal"
```

##幅(layout_width)、高さ(layout_height)の指定
match_parent: 親要素の幅に合わせる  
wrap_content: 中身（テキスト）の幅に合わせる  
任意の数値：nndp

```
    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="hello world hello world" />
    <Button
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="Hello world" />
    <Button
        android:layout_width="160dp"
        android:layout_height="160dp"
        android:text="Hello world" />
    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello world" />
```

##余白と寄せ方
余白  

* android:layout_margin  
* android:padding  

寄せ方  

* android:gravity  
* android:layout_gravity  


```
    <Button
        android:layout_margin="80dp"
        android:gravity="bottom"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="@string/hello_world" />
    <Button
        android:layout_marginBottom="80dp"
        android:layout_marginLeft="40dp"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="@string/hello_world" />
    <Button
        android:padding="40dp"
        android:layout_gravity="right"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="@string/hello_world" />
    <Button
        android:paddingBottom="40dp"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="@string/hello_world" />
```