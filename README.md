<h1 align="center">
  MyLibStyle
</h1>

<div align="center">
    <a><img src="https://img.shields.io/badge/Version-0.0.8-brightgreen.svg?style=flat"></a>
    <a><img src="https://img.shields.io/badge/ID-gzeinnumer-blue.svg?style=flat"></a>
    <a><img src="https://img.shields.io/badge/Java-Suport-green?logo=java&style=flat"></a>
    <a><img src="https://img.shields.io/badge/Koltin-Suport-green?logo=kotlin&style=flat"></a>
    <a href="https://github.com/gzeinnumer"><img src="https://img.shields.io/github/followers/gzeinnumer?label=follow&style=social"></a>
    <br>
    <p>Simple way to use Material.io</p>
</div>

---

**FullExample.**
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/example1.jpg)|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/example2.jpg)|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/example3.jpg)|
|--|--|--|

---

## Download
Add maven `jitpack.io` and `dependencies` in `build.gradle (Project)` :
```gradle
// build.gradle project
allprojects {
  repositories {
    ...
    maven { url 'https://jitpack.io' }
  }
}

// build.gradle app/module
dependencies {
  ...
  implementation 'com.github.gzeinnumer:MyLibStyle:version'
}
```

## Feature List
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
- [x] Dialog ([DOCS](https://github.com/gzeinnumer/MyLibDialog))

## Tech stack and 3rd library
- Material.io ([docs](https://material.io/develop/android/docs/getting-started))

---

**First Step**. Use `MaterialComponents` in `style.xml` with change parent of `AppTheme` :

```xml
<style name="AppTheme" parent="Theme.MaterialComponents.Light.NoActionBar">
    <!-- Customize your theme here. -->
</style>
```

**Notes. You can custom all style, example :**

Default from MyLibStyle :
```xml
<TextView
    style="@style/MyTextHeader"
    android:text="MyTextHeader" />

<TextView
    style="@style/MyTextContent"
    android:text="MyTextContent" />
```

Own Custom :
```xml
<TextView
    style="@style/MyTextHeader"
    android:text="MyTextHeader" />

<TextView
    style="@style/MyTextContent"
    android:text="MyTextContent"
    android:textColor="@android:color/holo_red_dark"
    android:textSize="36sp" />
```
Preview:

|<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/2.MyTextContent_3.jpg" width="400"/>|<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/2.MyTextContent_2.jpg" width="400"/>|
|--|--|
|Default|Custom|

---
## USE

**MyAppbarLayout.**
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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/_1.MyCustomToolbarTitle.jpg" width="400"/>
</p>

#

**MyTopHeader.**
```xml
<TextView
    android:id="@+id/tv_title"
    style="@style/MyTopHeader"
    android:text="MyTopHeader : MainActivity" />
```
Preview:
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/_1.MyTopHeader.jpg" width="400"/>
</p>

#

**MyTextHeader.**
```xml
<TextView
    style="@style/MyTextHeader"
    android:text="MyTextHeader" />
```
Preview:
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/1.MyTextHeader.jpg" width="400"/>
</p>

#

**MyTextContent.**
```xml
<TextView
    style="@style/MyTextContent"
    android:text="MyTextContent" />
```
Preview:
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/2.MyTextContent.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/3.MyTextIputLayoutOutlinedBox_Pass.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/4.MyTextIputLayoutOutlinedBoxNext.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/5.MyTextIputLayoutOutlinedBoxNext_Man.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/6.MyTextIputLayoutFilledBox.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/7.MyTextIputLayoutFilledBoxNext_Icon.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/8.MyTextIputLayoutOutlinedBoxNext_Helper.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/9.MyTextIputLayoutFilledBox_Man.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/10.MyButtonOutlined.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/11.MyButtonText.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/12.MyButtonContained.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/13.MyButtonIcon.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/14.MyAutoCompleteTextViewFilledBox.jpg" width="400"/>
</p>

OnClick:
|<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/14.MyAutoCompleteTextViewFilledBox_Example.jpg" width="400"/>|<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/14.MyAutoCompleteTextViewFilledBox_Example_2.jpg" width="400"/>|
|--|--|

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/15.MyAutoCompleteTextViewOutlinedBox.jpg" width="400"/>
</p>

OnClick:
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/15.MyAutoCompleteTextViewOutlinedBox_Example.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/16.Dialog.jpg" width="400"/>
</p>

OnClick:
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/16.Dialog_Example.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/17.Dropdown.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/18.TextRequired.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/19.TakeFoto.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/20.IconImage.jpg" width="400"/>
</p>

#

**MyDivider.**
```xml
<View style="@style/MyDivider" />
```
Preview:
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/21.MyDivider.jpg" width="400"/>
</p>

#

**MyRadioGroup.**
```xml
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
```
Preview:
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/23.MyRadioButton.jpg" width="400"/>
</p>

#

**MyRadioGroup.**
```xml
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
```
Preview:
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/24.MyRadioButton_Horizontal.jpg" width="400"/>
</p>

#

**MyRadioGroup.**
```xml
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
```
Preview:
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/25.MyRadioButton_Horizontal_Title.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/26.MyTextEditText.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/28.MyEditText_Horizontal.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/29.MyCheckBoxText.jpg" width="400"/>
</p>

#

**MyCheckBox_Horizontal.**
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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/31.MyCheckBox_Horizontal.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/31.MyCheckBox_Horizontal.jpg" width="400"/>
</p>

#

**MyBottomNavigationView.**
```xml
<com.google.android.material.bottomnavigation.BottomNavigationView
    android:id="@+id/btn_nav"
    style="@style/MyBottomNavigationView"
    app:menu="@menu/mygzn_bottom_nav" />
```
Preview:
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/32.ButtonNav.jpg" width="400"/>
</p>

#

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
<p align="center">
<img src="https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/33.MyParentTypeCardEdge.jpg" width="400"/>
</p>

---

### Version
- **0.0.3**
  - First Release
- **0.0.6**
  - Font Style
- **0.0.7**
  - Icon Foto
- **0.0.8**
  - Add More Style

---

### Contribution
You can sent your constibution to `branche` `open-pull`.

---

```
Copyright 2020 M. Fadli Zein
```

