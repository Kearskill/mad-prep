Location Permission

```xml
<manifest>
    <uses-permission android:name="android.permission,ACCESS_BACKGROUND_LOCATION"/>
</manifest>
```


Accuracy (Coarse Location or Fine Location)

```xml
<manifest>
    <uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION"/>
    
    <uses-permission android:name="android.permission.ACCESS_FINE_LOCATION"/>
</manifest>
```

Add Maps

```java
SupportMapFragment mapFragment = SupportMapFragment.newInstance();
getSupportFragmentManager()
    .beginTransaction()
    .add(R.id.my_container, mapFragment)
    .commit();
```

