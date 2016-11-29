### I. Java style

First should follow Android Coding Style
https://source.android.com/source/code-style.html#fully-qualify-imports


#### #Class Property order
1. Constants
2. Fields
3. Constructors
4. Override methods and callbacks (public or private)
5. Public methods
6. Private methods
7. Inner classes or interfaces

#### #Activity lifecycle function order
```java
public class MainActivity extends Activity {
    
    @Override 
    public void onCreate() {} 

    @Override 
    public void onResume() {}

    @Override 
    public void onPause() {}

    @Override 
    public void onDestory() {}
}
```
#### #Function argument order
```java
// Context should always place at first
public User loadUser(Context context, int userId);

// Callbacks should always place at last
public void loadUserAsync(Context context, int userId, UserCallback callback);
```

#### #For xml mapped naming

| Layout               | Prefix              | Example              |
| -----------------    | -----------------   | -----------------   |
| `TextView`          | `tv`            | `tvTitle`            | 
| `ImageView`          | `btn`            |`btnOk`            | 
| `ImageView`          | `iv`            |`ivAvatar`            | 
| `EditText`          | `edt`            |
| `RecyclerView`          | `rv`            |
| `Progressbar`          | `pgb`            | 
| `RadioButton`          | `rd`            | 
| `RadioButton`          | `rg`            | 
| `LinearLayout`          | `ll`            | 
| `RelativeLayout`          | `rl`            |
| `FrameLayout`          | `fl`            |


### Use Log

Every class should have a default variable TAG
```java
public class MyClass {
    private static final String TAG = "MyClass";

    public myMethod() {
        Log.e(TAG, "Error message");
    }
}
```
### II. Resource Style

#### #Layout naming
Use lowercase_underscore

| Layout               | Prefix              | Example              |
| -----------------    | -----------------   |-----------------   |
| `Activity`           | `activity_`             | `activity_main`             |
| `Fragment`          | `fragment_`            | 
| `Dialog`          | `dialog_`            | 
| `RecyclerView List Items`          | `item_list_`            | 
| `RecyclerView Grid Items`          | `item_grid_`            | 
| `Another Layout`          | `layout_`            | 

#### #ID Naming

| Element              | Prefix              |
| -----------------    | -----------------   |
| `TextView`           | `text_`             |
| `EditText`           | `edit_text_`             |
| `ImageView`          | `image_`            | 
| `Button`             | `button_`           |   
| `Menu`               | `menu_`             |
| `RelativeLayout`     | `relative_`         |
| `LinearLayout `      | `linear_`           |
| `ProgressBar `      | `progress_`           |


```xml

<ImageView
    android:id="@+id/image_profile"/>

```

#### #Drawable resource naming

| State        | Suffixes        | Example                     |
|--------------|-----------------|-----------------------------|
| Normal       | `_normal`       | `button_ok_normal.png`    |
| Pressed      | `_pressed`      | `button_ok_pressed.png`   |
| Focused      | `_focused`      | `button_ok_focused.png`   |
| Disabled     | `_disabled`     | `button_ok_disabled.png`  |
| Selected     | `_selected`     | `button_ok_selected.png`  |

#### #Strings

#####For short text: use lowercase_underscore

```xml

<string name="first_name">First Name</string>

```

#####For long text, use prefix like

| Prefix             | Description                           |
| -----------------  | --------------------------------------|
| `error_`           | For error message                   |
| `msg_`             | For notification or message        |       
| `hint_`            | For hint/placeholder         | 
| `text_`            | For long text/description  |


#### #Menu

Menu name should follow `activity` or `fragment` name
Example: `MainActivity` => `menu_main`

#### #Styles and Themes

Uppercase first letter

```xml

<style name="TextHeader"></style>

```

#### #Dimens

Choose one layout type as a standar layout (for example: values-360dp)

| Prefix             | Description                           |
| -----------------  | --------------------------------------|
| `dp_`              | For dp                                |
| `sp_`              | For sp                                |        
| `dp_*_negative`    | For negative value                    | 

```xml

<dimens name="dp_10">10dp</dimens>
<dimens name="sp_10">10sp</dimens>
<dimens name="dp_10_negative">-10dp</dimens>

```


#### #XML end tags
Should
```xml
<TextView
    android:layout_width="wrap_content"
    android:layout_height="wrap_content" />
```
Shouldn't
```xml
<TextView
    android:layout_width="wrap_content"
    android:layout_height="wrap_content">
</TextView>
```
#### #Attribute order (suggest: always use AndroiStudio format)

1. View Id
2. Style
3. Layout width and layout height
4. Other layout attributes, sorted alphabetically
