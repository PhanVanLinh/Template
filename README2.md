
### 3.2 Resources naming

Use lowercase_underscore

#### 3.2.1 ID Naming

ID

| Element              | Prefix              |
| -----------------    | -----------------   |
| `TextView`           | `text_`             |
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

#### 3.2.2 Strings

#For short text: use lowercase_underscore


```xml

<string name="first_name">First Name</string>

```

#For long text, use prefix like

| Prefix             | Description                           |
| -----------------  | --------------------------------------|
| `error_`           | For error message                   |
| `msg_`             | For notification or message        |       
| `hint_`            | For hint/placeholder         | 
| `text_`            | For long text/description  |

#### 3.2.3 Styles and Themes

Uppercase first letter

```xml

<style name="TextHeader"></style>

```

#### 3.2.4 Attribute order (suggest: always use AndroiStudio format)

1. View Id
2. Style
3. Layout width and layout height
4. Other layout attributes, sorted alphabetically