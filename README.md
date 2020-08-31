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
Code:
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

**MyTextHeader.**
Code:
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
---

```
Copyright 2020 M. Fadli Zein
```

