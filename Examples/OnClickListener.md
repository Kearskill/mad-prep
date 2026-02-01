OnClickListener

```xml
<Button
    android:id="@+id/BtnUseListener"
    android:layout_width="wrap_content"
    android:layout_height = "wrap_content"
    android:text="Use Listener"/>
```


```java
@Override
protected void onCreate(Bundle savedInstanceState){
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
    
    Button UseListenerBtn = (Button) findViewById(R.id.BtnUseListener);
}

private View.OnClickListener ButtonOnClickListener = new View.OnClickListener(){
    @Override
    public void onClick(View view){
        Context context = getApplicationContext();
        String text = "Hello twin";
        int duration = Toast.LENGTH_LONG;
        
        Toast popupmessage = Toast.makeText(context, text, duration);
        popupmessage.show();
    }
};
```

