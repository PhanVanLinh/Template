### 3.2 Java naming
Use camel case

For xml mapped
| Xml               | Prefix               | Example              |
| -----------------    | -----------------   | -----------------   |
| `Button`           | `btn`             | `btnOk`             | 
| `TextView`          | `tv`            | 
| `ImageView`          | `iv`            |
| `EditText`          | `edt`            |
| `RecyclerView`          | `rv`            |
| `Progressbar`          | `pgb_`            | 
| `RadioButton`          | `rd_`            | 
| `RadioButton`          | `rg_`            | 
| `LinearLayout`          | `ll`            | 
| `RelativeLayout`          | `rl`            |
| `FrameLayout`          | `fl`            |


### 3.2 Layout resource naming


| Layout               | Prefix              |
| -----------------    | -----------------   |
| `Activity`           | `activity_`             |
| `Fragment`          | `fragment_`            | 
| `Dialog`          | `dialog_`            | 
| `RecyclerView Items`          | `item_`            | 
| `Another Layout`          | `layout_`            | 

### 3.2 Resources naming

Use lowercase_underscore

#### #ID Naming

ID

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

#### #Attribute order (suggest: always use AndroiStudio format)

1. View Id
2. Style
3. Layout width and layout height
4. Other layout attributes, sorted alphabetically
