<h1 align="center">
  MyLibStyle
</h1>

<div align="center">
    <a><img src="https://img.shields.io/badge/Version-0.0.3-brightgreen.svg?style=flat"></a>
    <a><img src="https://img.shields.io/badge/ID-gzeinnumer-blue.svg?style=flat"></a>
    <a href="https://github.com/gzeinnumer"><img src="https://img.shields.io/github/followers/gzeinnumer?label=follow&style=social"></a>
    <p>Kumpulan Style siap pakai yang sering dipakai di development android dengan material.io, tujuan library ini hanya untuk menghilangkan pengulangan kode pada xml, jadi kamu bisa lebih fokus pada logika, dokumen ini dibuat berdasarkan pengalaman saya, kasih masukan kalau ada yang kurang. terimakasih karna sudah berkunjung</p>
</div>

---

### Feature List
- [x] TextView
- [x] TextInputLayout
- [x] TextInputEditText
- [x] Divider
- [x] ButtonOutLined
- [x] ButtonText
- [x] ButtonIcon
- [x] ButtonContained
- [x] AutoCompleteTextView
- [x] TakeFotoIcon
- [x] ImagePreview
- [x] RadioGroup
- [x] RadioButton
- [x] CheckBox
- [x] ButtonNavigation
- [x] HomeBackIcon
- [x] TitleActionBar
- [x] ActionBarMenuIcon
- [x] ActionBarMenuText
- [x] SearchSpinner
- [x] Corner
- [x] Popup
- [ ] Dialog

---

### Tech stack and 3rd library
- Material.io ([docs](https://material.io/develop/android/docs/getting-started))

---

## Download

Minimum Android SDK Version 16

#### Gradle
**Step 1.** tambahkan maven jitpack.io ke build.gradle (Project) :
```gradle
allprojects {
  repositories {
    google()
    jcenter()
    maven { url 'https://jitpack.io' }
  }
}
```

**Step 2.** tambahkan depedensi ke build.gradle (Module) :
```gradle
dependencies {
  implementation 'com.github.gzeinnumer:MyLibStyle:versi'
}
```

---

**MyTextHeader.**
```xml
<com.google.android.material.appbar.AppBarLayout
    android:id="@+id/apb"
    style="@style/MyAppbarLayout">

    <com.google.android.material.appbar.MaterialToolbar
        android:id="@+id/tb"
        style="@style/MyMaterialToolbar">

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content">

            <ImageButton
                android:id="@+id/btn_back"
                style="@style/MyCostumToolbarImage"
                android:src="@drawable/mygzn_keyboard_arrow_left"
                android:tag="CostumToolbarImage" />

            <TextView
                android:id="@+id/tv_toolbar"
                style="@style/MyCostumToolbarTitle"
                android:text="MyCostumToolbarTitle" />

            <ImageButton
                android:id="@+id/btn_popup"
                style="@style/MyOptionMenu"
                android:src="@drawable/mygzn_more_vert" />
        </LinearLayout>
    </com.google.android.material.appbar.MaterialToolbar>
</com.google.android.material.appbar.AppBarLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/_1.MyCustomToolbarTitle.jpg)|
|--|
|MyAppbarLayout->
background:transparent 
elevation:0dp
MyAppbarLayout->
layout_width:match_parent 
layout_height:?actionBarSize
contentInsetLeft:0dp
contentInsetStart:0dp
MyCostumToolbarImage->
backgroundTint:transparent 
layout_width:24dp 
layout_height:24dp
layout_marginStart:10dp
layout_marginTop:10dp
layout_marginBottom:10dp
MyCostumToolbarTitle->
textAlignment:center
textStyle:bold
layout_weight:1
textSize:18dp
layout_marginStart:10dp
layout_marginTop:10dp
layout_marginBottom:10dp
MyOptionMenu->
backgroundTint:transparent
layout_width:24dp 
layout_height:24dp
layout_marginStart:10dp
layout_marginTop:10dp
layout_marginBottom:10dp
layout_marginEnd:10dp|
<br>

---

**MyTextHeader.**
```xml
<TextView
    android:id="@+id/tv_title"
    style="@style/MyTopHeader"
    android:text="MyTopHeader : MainActivity" />
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/_1.MyTopHeader.jpg)|
|--|
|MyAppbarLayout->
layout_width:match_parent 
layout_height:40dp
gravity:center
textColor:#000
textSize:16sp|
<br>

---

**MyTextHeader.**
```xml
<TextView
    style="@style/MyTextHeader"
    android:text="MyTextHeader" />
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/1.MyTextHeader.jpg)|
|--|
|textStyle:bold 
textSize:16sp
layout_marginTop:10dp|
<br>

---

**MyTextContent.**
```xml
<TextView
    style="@style/MyTextContent"
    android:text="MyTextContent" />
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/2.MyTextContent.jpg)|
|--|
|textStyle:bold 
textSize:16sp|
<br>

---

**MyTextInputLayoutOutlinedBox.**
```xml
<com.google.android.material.textfield.TextInputLayout
    style="@style/MyTextInputLayoutOutlinedBox"
    android:hint="MyTextInputLayoutOutlinedBox"
    app:endIconMode="password_toggle">

    <com.google.android.material.textfield.TextInputEditText
        android:id="@+id/ed_1"
        style="@style/MyTextInputEditText"
        android:inputType="textPassword" />

</com.google.android.material.textfield.TextInputLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/3.MyTextIputLayoutOutlinedBox_Pass.jpg)|
|--|
|TextInputLayout->
layout_marginTop:10dp 
MyTextInputEditText->
textSize:16sp|
<br>

---

**MyTextInputLayoutOutlinedBoxNext.**
```xml
<com.google.android.material.textfield.TextInputLayout
    style="@style/MyTextInputLayoutOutlinedBoxNext"
    android:hint="MyTextInputLayoutOutlinedBoxNext">

    <com.google.android.material.textfield.TextInputEditText
        android:id="@+id/ed_2"
        style="@style/MyTextInputEditText" />

</com.google.android.material.textfield.TextInputLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/4.MyTextIputLayoutOutlinedBoxNext.jpg)|
|--|
|TextInputLayout->
layout_marginTop:10dp 
MyTextInputEditText->
textSize:16sp|
<br>

---

**MyTextInputLayoutOutlinedBoxNext.**
```xml
<com.google.android.material.textfield.TextInputLayout
    style="@style/MyTextInputLayoutOutlinedBoxNext"
    android:hint="MyTextInputLayoutOutlinedBoxNext*"
    android:textColorHint="@color/red_500">

    <com.google.android.material.textfield.TextInputEditText
        android:id="@+id/ed_7"
        style="@style/MyTextInputEditText" />

</com.google.android.material.textfield.TextInputLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/5.MyTextIputLayoutOutlinedBoxNext_Man.jpg)|
|--|
|TextInputLayout->
layout_marginTop:10dp 
MyTextInputEditText->
textSize:16sp|
<br>

---

**MyTextInputLayoutFilledBox.**
```xml
<com.google.android.material.textfield.TextInputLayout
    style="@style/MyTextInputLayoutFilledBox"
    android:hint="MyTextInputLayoutFilledBox">

    <com.google.android.material.textfield.TextInputEditText
        android:id="@+id/ed_3"
        style="@style/MyTextInputEditText" />

</com.google.android.material.textfield.TextInputLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/6.MyTextIputLayoutFilledBox.jpg)|
|--|
|TextInputLayout->
layout_marginTop:10dp 
MyTextInputEditText->
textSize:16sp|
<br>

---

**MyTextInputLayoutFilledBoxNext.**
```xml
<com.google.android.material.textfield.TextInputLayout
    style="@style/MyTextInputLayoutFilledBoxNext"
    android:hint="MyTextInputLayoutFilledBoxNext"
    app:startIconDrawable="@drawable/mygzn_home">

    <com.google.android.material.textfield.TextInputEditText
        android:id="@+id/ed_4"
        style="@style/MyTextInputEditText" />

</com.google.android.material.textfield.TextInputLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/7.MyTextIputLayoutFilledBoxNext_Icon.jpg)|
|--|
|TextInputLayout->
layout_marginTop:10dp 
MyTextInputEditText->
textSize:16sp|
<br>

---

**MyTextInputLayoutOutlinedBoxNext.**
```xml
<com.google.android.material.textfield.TextInputLayout
    style="@style/MyTextInputLayoutOutlinedBoxNext"
    android:hint="MyTextInputLayoutOutlinedBoxNext"
    app:counterEnabled="true"
    app:counterMaxLength="20"
    app:errorEnabled="true"
    app:helperText="Helper Text"
    app:helperTextEnabled="true">

    <com.google.android.material.textfield.TextInputEditText
        android:id="@+id/ed_5"
        style="@style/MyTextInputEditText" />

</com.google.android.material.textfield.TextInputLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/8.MyTextIputLayoutOutlinedBoxNext_Helper.jpg)|
|--|
|TextInputLayout->
layout_marginTop:10dp 
MyTextInputEditText->
textSize:16sp|
<br>

---

**MyTextInputLayoutFilledBox.**
```xml
<com.google.android.material.textfield.TextInputLayout
    style="@style/MyTextInputLayoutFilledBox"
    android:hint="MyTextInputLayoutFilledBox*"
    android:textColorHint="@color/red_500">

    <com.google.android.material.textfield.TextInputEditText
        android:id="@+id/ed_6"
        style="@style/MyTextInputEditText" />

</com.google.android.material.textfield.TextInputLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/9.MyTextIputLayoutFilledBox_Man.jpg)|
|--|
|TextInputLayout->
layout_marginTop:10dp 
MyTextInputEditText->
textSize:16sp|
<br>

---

**MyButtonOutlined.**
```xml
<LinearLayout
    style="@style/MyParentButton"
    android:gravity="end"
    android:orientation="vertical">

    <Button
        style="@style/MyButtonOutlined"
        android:text="MyButtonOutlined" />

</LinearLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/10.MyButtonOutlined.jpg)|
|--|
|MyParentButton->
layout_marginTop:10dp 
MyButtonOutlined->
layout_height:48dp|
<br>

---

**MyButtonText.**
```xml
<LinearLayout
    style="@style/MyParentButton"
    android:gravity="end"
    android:orientation="vertical">

    <Button
        style="@style/MyButtonText"
        android:text="MyButtonText" />

</LinearLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/11.MyButtonText.jpg)|
|--|
|MyParentButton->
layout_marginTop:10dp 
MyButtonText->
layout_height:48dp|
<br>

---

**MyButtonContained.**
```xml
<LinearLayout
    style="@style/MyParentButton"
    android:gravity="end"
    android:orientation="vertical">

    <Button
        style="@style/MyButtonContained"
        android:text="MyButtonContained" />

</LinearLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/12.MyButtonContained.jpg)|
|--|
|MyParentButton->
layout_marginTop:10dp 
MyButtonContained->
layout_height:48dp|
<br>

---

**MyButtonIcon.**
```xml
<LinearLayout
    style="@style/MyParentButton"
    android:gravity="end"
    android:orientation="vertical">

    <Button
        style="@style/MyButtonIcon"
        android:text="MyButtonIcon"
        app:icon="@drawable/mygzn_add" />

</LinearLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/13.MyButtonIcon.jpg)|
|--|
|MyParentButton->
layout_marginTop:10dp 
MyButtonIcon->
layout_height:48dp|
<br>

---

**MyAutoCompleteTextViewFilledBox.**
```xml
<com.google.android.material.textfield.TextInputLayout
    style="@style/MyAutoCompleteTextViewFilledBox"
    android:hint="MyAutoCompleteTextViewFilledBox">

    <AutoCompleteTextView
        android:id="@+id/material_spinner_1"
        style="@style/MyAutoCompleteTextView" />

</com.google.android.material.textfield.TextInputLayout>
```

```kotlin
val items = listOf("Mercury", "Venus", "Earth", "Mars", "Jupiter", "Saturn", "Uranus", "Neptune")
val myAdapter = ArrayAdapter(applicationContext, R.layout.mygzn_list_item, items)
material_spinner_1.setAdapter(myAdapter)
```

Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/14.MyAutoCompleteTextViewFilledBox.jpg)|
|--|
|MyAutoCompleteTextViewFilledBox->
layout_marginTop:10dp 
MyAutoCompleteTextView->
editable:false
inputType:none
textSize:16sp|

OnClick:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/14.MyAutoCompleteTextViewFilledBox_Example.jpg)|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/14.MyAutoCompleteTextViewFilledBox_Example_2.jpg)|
|--|--|
<br>

---

**MyAutoCompleteTextViewOutlineBox.**
```xml
<com.google.android.material.textfield.TextInputLayout
    style="@style/MyAutoCompleteTextViewOutlineBox"
    android:hint="MyAutoCompleteTextViewOutlineBox">

    <AutoCompleteTextView
        android:id="@+id/material_spinner_2"
        style="@style/MyAutoCompleteTextView" />

</com.google.android.material.textfield.TextInputLayout>
```

```kotlin
val items = listOf("Mercury", "Venus", "Earth", "Mars", "Jupiter", "Saturn", "Uranus", "Neptune")
val myAdapter = ArrayAdapter(applicationContext, R.layout.mygzn_list_item, items)
material_spinner_2.setAdapter(myAdapter)
```

Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/15.MyAutoCompleteTextViewOutlinedBox.jpg)|
|--|
|MyAutoCompleteTextViewOutlineBox->
layout_marginTop:10dp 
MyAutoCompleteTextView->
editable:false
inputType:none
textSize:16sp|

OnClick:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/15.MyAutoCompleteTextViewOutlinedBox_Example.jpg)|
|--|

<br>

---

**MySpinner.**
```xml
<LinearLayout style="@style/MyParentSpinner">

    <TextView
        style="@style/MyTextContent"
        android:layout_weight="1"
        android:text="Dialog" />

    <Spinner
        android:id="@+id/material_spinner_4"
        style="@style/MySpinner"
        android:layout_weight="1"
        android:prompt="@string/app_name"
        android:spinnerMode="dialog" />

</LinearLayout>
```

```kotlin
val items = listOf("Mercury", "Venus", "Earth", "Mars", "Jupiter", "Saturn", "Uranus", "Neptune")
val myAdapter = ArrayAdapter(applicationContext, R.layout.mygzn_list_item, items)
material_spinner_4.adapter = myAdapter
```

Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/16.Dialog.jpg)|
|--|
|MyParentSpinner->
layout_marginTop:10dp|

OnClick:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/16.Dialog_Example.jpg)|
|--|
<br>

---

**MySpinner.**
```xml
<LinearLayout style="@style/MyParentSpinner">

    <TextView
        style="@style/MyTextContent"
        android:layout_weight="1"
        android:text="Dropdown" />

    <androidx.appcompat.widget.AppCompatSpinner
        android:id="@+id/material_spinner_5"
        style="@style/MySpinner"
        android:layout_weight="1"
        android:prompt="@string/app_name"
        android:spinnerMode="dropdown" />

</LinearLayout>
```

```kotlin
val items = listOf("Mercury", "Venus", "Earth", "Mars", "Jupiter", "Saturn", "Uranus", "Neptune")
val myAdapter = ArrayAdapter(applicationContext, R.layout.mygzn_list_item, items)
material_spinner_5.adapter = myAdapter
```

Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/17.Dropdown.jpg)|
|--|
|MyParentSpinner->
layout_marginTop:10dp|

OnClick:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/17.Dropdown_Example.jpg)|
|--|
<br>

---

**MyImageFoto.**
```xml
<LinearLayout
    android:id="@+id/img_1"
    style="@style/MyImageFoto"
    android:layout_width="match_parent">

    <TextView
        style="@style/MyTextRequired"
        android:layout_gravity="center" />

    <ImageView
        style="@style/MyTakeImage"
        android:src="@drawable/mygzn_take_image" />

    <TextView style="@style/MyImageFotoText" />

</LinearLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/18.TextRequired.jpg)|
|--|
|MyImageFoto->
layout_marginTop:10dp
paddingStart:8dp
paddingEnd:8dp
gravity:center
orientation:vertical
MyTextRequired->
text:*Required
textStyle:italic
textSize:11sp
textColor:#F44336
MyImageFotoText->
text:Take Foto
textStyle:itelic
textSize:11sp|
<br>

---

**MyImageFoto.**
```xml
<LinearLayout
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:gravity="center">

    <LinearLayout
        android:id="@+id/img_2"
        style="@style/MyImageFoto">

        <ImageView
            style="@style/MyTakeImage"
            android:src="@drawable/mygzn_take_image" />

        <TextView style="@style/MyImageFotoText" />

    </LinearLayout>

    <LinearLayout
        android:id="@+id/img_3"
        style="@style/MyImageFoto">

        <ImageView
            style="@style/MyTakeImage"
            android:src="@drawable/mygzn_take_image" />

        <TextView style="@style/MyImageFotoText" />

    </LinearLayout>

    <LinearLayout
        android:id="@+id/img_4"
        style="@style/MyImageFoto">

        <ImageView
            style="@style/MyTakeImage"
            android:src="@drawable/mygzn_take_image" />

        <TextView style="@style/MyImageFotoText" />

    </LinearLayout>
</LinearLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/19.TextFoto.jpg)|
|--|
|MyImageFoto->
layout_marginTop:10dp
paddingStart:8dp
paddingEnd:8dp
gravity:center
orientation:vertical
MyImageFotoText->
text:Take Foto
textStyle:itelic
textSize:11sp|
<br>

---

**MyImageFoto.**
```xml
<LinearLayout
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:layout_marginTop="@dimen/space_between_photo_preview"
    android:gravity="center">

    <ImageView style="@style/MyImageFotoPreview" />

    <ImageView
        style="@style/MyImageFotoPreview"
        android:src="@drawable/mygzn_gzeinnumer_crop" />

</LinearLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/20.IconImage.jpg)|
|--|
|MyImageFotoPreview->
layout_margin:8dp
layout_width:70dp
layout_height:70dp
layout_gravity:center|
<br>

---

**MyDivider.**
```xml
<View style="@style/MyDivider" />
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/21.MyDivider.jpg)|
|--|
|MyDivider->
layout_height:0.8dp
layout_marginTop:10dp|
<br>

---

**MyRadioGroup.**
```xml
<LinearLayout
    style="@style/MyParentRadioGroup"
    android:orientation="vertical">

    <TextView
        style="@style/MyTextHeader"
        android:text="MyTextHeader" />

    <TextView
        style="@style/MyRadioGroupText"
        android:text="MyRadioGroupText" />

    <RadioGroup
        android:id="@+id/rg"
        style="@style/MyRadioGroup"
        android:checkedButton="@+id/first">

        <RadioButton
            android:id="@+id/first"
            style="@style/MyRadioButton"
            android:text="MyRadioButton" />

        <RadioButton
            android:id="@+id/second"
            style="@style/MyRadioButton"
            android:text="MyRadioButton" />
    </RadioGroup>

    <TextView
        style="@style/MyRadioGroupText"
        android:text="MyRadioGroupText" />

    <RadioGroup
        android:id="@+id/rg_1"
        style="@style/MyRadioGroup"
        android:checkedButton="@+id/first_1"
        android:orientation="horizontal">

        <RadioButton
            android:id="@+id/first_1"
            style="@style/MyRadioButton"
            android:text="MyRadioButton" />

        <RadioButton
            android:id="@+id/second_1"
            style="@style/MyRadioButton"
            android:text="MyRadioButton" />
    </RadioGroup>

    <View style="@style/MyDivider" />

    <TextView
        style="@style/MyTextHeader"
        android:text="MyTextHeader" />

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:gravity="center_vertical">

        <TextView
            style="@style/MyTextContent"
            android:layout_gravity="center|left"
            android:layout_marginTop="3dp"
            android:layout_weight="1"
            android:text="MyTextContent" />

        <RadioGroup
            android:id="@+id/rg_2"
            style="@style/MyRadioGroup"
            android:layout_weight="1"
            android:checkedButton="@+id/first_2"
            android:orientation="horizontal">

            <RadioButton
                android:id="@+id/first_2"
                style="@style/MyRadioButton"
                android:text="MyRadioButton" />

            <RadioButton
                android:id="@+id/second_2"
                style="@style/MyRadioButton"
                android:text="MyRadioButton" />
        </RadioGroup>
    </LinearLayout>
</LinearLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/23.MyRadioButton.jpg)|
|--|
|MyParentRadioGroup->
layout_marginTop:10dp
MyParentRadioGroup->
layout_marginTop:10dp
textSize:16sp
MyRadioGroup->
layout_marginTop:10dp
textSize:16sp
orientation:vertical
layout_weight:1
paddingStart:-5dp
MyRadioButton->
textSize:16sp|
<br>

---

**MyRadioGroup.**
```xml
<LinearLayout
    style="@style/MyParentRadioGroup"
    android:orientation="vertical">

    <TextView
        style="@style/MyTextHeader"
        android:text="MyTextHeader" />

    <TextView
        style="@style/MyRadioGroupText"
        android:text="MyRadioGroupText" />

    <RadioGroup
        android:id="@+id/rg"
        style="@style/MyRadioGroup"
        android:checkedButton="@+id/first">

        <RadioButton
            android:id="@+id/first"
            style="@style/MyRadioButton"
            android:text="MyRadioButton" />

        <RadioButton
            android:id="@+id/second"
            style="@style/MyRadioButton"
            android:text="MyRadioButton" />
    </RadioGroup>

    <TextView
        style="@style/MyRadioGroupText"
        android:text="MyRadioGroupText" />

    <RadioGroup
        android:id="@+id/rg_1"
        style="@style/MyRadioGroup"
        android:checkedButton="@+id/first_1"
        android:orientation="horizontal">

        <RadioButton
            android:id="@+id/first_1"
            style="@style/MyRadioButton"
            android:text="MyRadioButton" />

        <RadioButton
            android:id="@+id/second_1"
            style="@style/MyRadioButton"
            android:text="MyRadioButton" />
    </RadioGroup>

    <View style="@style/MyDivider" />

    <TextView
        style="@style/MyTextHeader"
        android:text="MyTextHeader" />

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:gravity="center_vertical">

        <TextView
            style="@style/MyTextContent"
            android:layout_gravity="center|left"
            android:layout_marginTop="3dp"
            android:layout_weight="1"
            android:text="MyTextContent" />

        <RadioGroup
            android:id="@+id/rg_2"
            style="@style/MyRadioGroup"
            android:layout_weight="1"
            android:checkedButton="@+id/first_2"
            android:orientation="horizontal">

            <RadioButton
                android:id="@+id/first_2"
                style="@style/MyRadioButton"
                android:text="MyRadioButton" />

            <RadioButton
                android:id="@+id/second_2"
                style="@style/MyRadioButton"
                android:text="MyRadioButton" />
        </RadioGroup>
    </LinearLayout>
</LinearLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/24.MyRadioButton_Horizontal.jpg)|
|--|
|MyParentRadioGroup->
layout_marginTop:10dp
MyParentRadioGroup->
layout_marginTop:10dp
textSize:16sp
MyRadioGroup->
layout_marginTop:10dp
textSize:16sp
orientation:vertical
layout_weight:1
paddingStart:-5dp
MyRadioButton->
textSize:16sp|
<br>

---

**MyRadioGroup.**
```xml
<LinearLayout
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:gravity="center_vertical">

    <TextView
        style="@style/MyTextContent"
        android:layout_gravity="center|left"
        android:layout_marginTop="3dp"
        android:layout_weight="1"
        android:text="MyTextContent" />

    <RadioGroup
        android:id="@+id/rg_2"
        style="@style/MyRadioGroup"
        android:layout_weight="1"
        android:checkedButton="@+id/first_2"
        android:orientation="horizontal">

        <RadioButton
            android:id="@+id/first_2"
            style="@style/MyRadioButton"
            android:text="MyRadioButton" />

        <RadioButton
            android:id="@+id/second_2"
            style="@style/MyRadioButton"
            android:text="MyRadioButton" />
    </RadioGroup>
</LinearLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/25.MyRadioButton_Horizontal_Title.jpg)|
|--|
|MyRadioGroup->
layout_marginStart:10dp
layout_marginEnd:-4dp
textSize:16sp|
<br>

---

**MyEditText.**
```xml
<TextView
    style="@style/MyTextEditText"
    android:text="MyTextEditText" />

<EditText
    style="@style/MyEditText"
    android:backgroundTint="@color/colorPrimary"
    android:hint="MyEditText" />
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/26.MyTextEditText.jpg)|
|--|
|MyTextEditText->
layout_marginTop:10dp
textSize:16sp
MyEditText->
layout_marginTop:-8dp
layout_marginStart:-4dp
layout_marginEnd:-4dp
textSize:16sp
inputType:textImeMultiLine
lines:3
minLines:3|
<br>

---

**MyEditText_Horizontal.**
```xml
<LinearLayout
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:layout_gravity="center_vertical">

    <TextView
        style="@style/MyTextContent"
        android:text="MyTextContent" />

    <EditText
        style="@style/MyEditText_Horizontal"
        android:layout_weight="1"
        android:hint="MyEditText_Horizontal" />
</LinearLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/28.MyEditText_Horizontal.jpg)|
|--|
|MyEditText_Horizontal->
layout_marginStart:10dp
layout_marginEnd:-4dp
textSize:16sp
inputType:textImeMultiLine
lines:3
minLines:3|
<br>

---

**MyCheckBox.**
```xml
<TextView
    style="@style/MyCheckBoxText"
    android:text="MyCheckBoxText" />

<com.google.android.material.checkbox.MaterialCheckBox
    style="@style/MyCheckBox"
    android:text="MyCheckBox" />
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/29.MyCheckBoxText.jpg)|
|--|
|MyCheckBoxText->
layout_marginTop:10dp
textSize:16sp
MyCheckBox->
layout_height:25dp
textSize:16sp
layout_marginStart:-7dp|
<br>

---

**MyCheckBox.**
```xml
<LinearLayout style="@style/MyParentCheckBox">

    <TextView
        style="@style/MyTextContent"
        android:text="MyTextContent" />

    <com.google.android.material.checkbox.MaterialCheckBox
        style="@style/MyCheckBox_Horizontal"
        android:text="MyCheckBox_Horizontal" />

</LinearLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/31.MyCheckBox_Horizontal.jpg)|
|--|
|MyParentCheckBox->
layout_marginTop:10dp
textSize:16sp
MyCheckBox_Horizontal->
layout_height:25dp
textSize:16sp
layout_marginStart:10dp|
<br>

---

**MyCheckBox.**
```xml
<com.google.android.material.bottomnavigation.BottomNavigationView
    android:id="@+id/btn_nav"
    style="@style/MyBottomNavigationView"
    app:menu="@menu/mygzn_bottom_nav" />
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/32.ButtonNav.jpg)|
|--|
|MyBottomNavigationView->
itemIconTint:#6200EE
itemTextColor:#6200EE|
<br>

---

**MyCheckBox.**
```xml
<LinearLayout style="@style/MyParentCheckBox">

    <TextView
        style="@style/MyTextContent"
        android:text="MyTextContent" />

    <com.google.android.material.checkbox.MaterialCheckBox
        style="@style/MyCheckBox_Horizontal"
        android:text="MyCheckBox_Horizontal" />

</LinearLayout>
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/31.MyCheckBox_Horizontal.jpg)|
|--|
|MyParentCheckBox->
layout_marginTop:10dp
textSize:16sp
MyCheckBox_Horizontal->
layout_height:25dp
textSize:16sp
layout_marginStart:10dp|
<br>

---

**MyCheckBox.**
```xml
<com.google.android.material.bottomnavigation.BottomNavigationView
    android:id="@+id/btn_nav"
    style="@style/MyBottomNavigationView"
    app:menu="@menu/mygzn_bottom_nav" />
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/32.ButtonNav.jpg)|
|--|
|MyBottomNavigationView->
itemIconTint:#6200EE
itemTextColor:#6200EE|
<br>

---

**MyParentTypeCardEdge.**
```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:focusableInTouchMode="true"
    android:orientation="vertical"
    tools:ignore="HardcodedText">

    <com.google.android.material.appbar.AppBarLayout
        android:id="@+id/apb"
        style="@style/MyAppbarLayout">

        <com.google.android.material.appbar.MaterialToolbar
            android:id="@+id/tb"
            style="@style/MyMaterialToolbar">

            <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="wrap_content">

                <ImageButton
                    android:id="@+id/btn_back"
                    style="@style/MyCostumToolbarImage"
                    android:src="@drawable/mygzn_keyboard_arrow_left"
                    android:tag="CostumToolbarImage" />

                <TextView
                    android:id="@+id/tv_toolbar"
                    style="@style/MyCostumToolbarTitle"
                    android:text="MyCostumToolbarTitle" />

                <ImageButton
                    android:id="@+id/btn_popup"
                    style="@style/MyOptionMenu"
                    android:src="@drawable/mygzn_more_vert" />
            </LinearLayout>
        </com.google.android.material.appbar.MaterialToolbar>
    </com.google.android.material.appbar.AppBarLayout>

    <LinearLayout
        style="@style/MyParentTypeCardEdge"
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:layout_weight="1">

        <!-- Your Widget -->

    </LinearLayout>

    <com.google.android.material.bottomnavigation.BottomNavigationView
        android:id="@+id/btn_nav"
        style="@style/MyBottomNavigationView"
        app:menu="@menu/mygzn_bottom_nav" />
</LinearLayout>
```

```kotlin
btn_popup.setOnClickListener {
    val popup = PopupMenu(this, btn_popup)
    val inflater: MenuInflater = popup.menuInflater
    inflater.inflate(R.menu.mygzn_bottom_nav, popup.menu)
    popup.setOnMenuItemClickListener { item ->
        when (item?.itemId) {
            R.id.id_next -> startActivity(Intent(applicationContext, MainActivity::class.java))
        }
        false
    }
    popup.show()
}
```

Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/33.MyParentTypeCardEdge.jpg)|
|--|
|MyAppbarLayout->
background:transparent 
elevation:0dp
MyAppbarLayout->
layout_width:match_parent 
layout_height:?actionBarSize
contentInsetLeft:0dp
contentInsetStart:0dp
MyCostumToolbarImage->
backgroundTint:transparent 
layout_width:24dp 
layout_height:24dp
layout_marginStart:10dp
layout_marginTop:10dp
layout_marginBottom:10dp
MyCostumToolbarTitle->
textAlignment:center
textStyle:bold
layout_weight:1
textSize:18dp
layout_marginStart:10dp
layout_marginTop:10dp
layout_marginBottom:10dp
MyOptionMenu->
backgroundTint:transparent
layout_width:24dp 
layout_height:24dp
layout_marginStart:10dp
layout_marginTop:10dp
layout_marginBottom:10dp
layout_marginEnd:10dp
MyParentTypeCardEdge->
padding:16dp
layout_marginLeft:16dp
layout_marginRight:16dp
layout_marginBottom:16dp
orientation:orientation
MyBottomNavigationView->
itemIconTint:#6200EE
itemTextColor:#6200EE|
<br>

---

**FullExample.**
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/example1.jpg)|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/example2.jpg)|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/example3.jpg)|
|--|--|--|
---

```
Copyright 2020 M. Fadli Zein
```

