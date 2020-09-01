<h1 align="center">
  MyLibStyle
</h1>

<div align="center">
    <a><img src="https://img.shields.io/badge/Version-0.0.2-brightgreen.svg?style=flat"></a>
    <a><img src="https://img.shields.io/badge/ID-gzeinnumer-blue.svg?style=flat"></a>
    <a href="https://github.com/gzeinnumer"><img src="https://img.shields.io/github/followers/gzeinnumer?label=follow&style=social"></a>
    <p>Kumpulan Style siap pakai yang sering dipakai di development android dengan material.io, dokumen ini dibuat berdasarkan pengalaman saya, kasih masukan kalau ada yang kurang. terimakasih karna sudah berkunjung</p>
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
- [X] Corner
- [ ] Dialog
- [ ] Popup

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
<TextView
    style="@style/MyTextHeader"
    android:text="MyTextHeader" />
```
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/1.MyTextHeader.jpg)|
|--|
|textStyle:bold 
textSize:16dp
layout_marginTop:10dp|
<br>

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
textSize:16dp|
<br>

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
textSize:16dp|
<br>

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
textSize:16dp|
<br>

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
textSize:16dp|
<br>

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
textSize:16dp|
<br>

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
textSize:16dp|
<br>

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
textSize:16dp|
<br>

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
textSize:16dp|
<br>

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
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/14.MyAutoCompleteTextViewFilledBox.jpg)|
|--|
|MyAutoCompleteTextViewFilledBox->
layout_marginTop:10dp 
MyAutoCompleteTextView->
editable:false
inputType:none
textSize:16dp|
<br>

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
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/15.MyAutoCompleteTextViewOutlinedBox.jpg)|
|--|
|MyAutoCompleteTextViewOutlineBox->
layout_marginTop:10dp 
MyAutoCompleteTextView->
editable:false
inputType:none
textSize:16dp|
<br>

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
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/16.Dialog.jpg)|
|--|
|MyParentSpinner->
layout_marginTop:10dp|
<br>

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
Preview:
|![](https://github.com/gzeinnumer/MyLibStyle/blob/master/assets/17.Dropdown.jpg)|
|--|
|MyParentSpinner->
layout_marginTop:10dp|
<br>


---

```
Copyright 2020 M. Fadli Zein
```

