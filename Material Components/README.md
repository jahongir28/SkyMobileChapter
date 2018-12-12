
Gradle dependencies

dependencies {
    implementation 'androidx.appcompat:appcompat:1.0.2'
    implementation 'androidx.legacy:legacy-support-v4:1.0.0'
    implementation 'com.google.android.material:material:1.1.0-alpha01'
    implementation 'androidx.constraintlayout:constraintlayout:2.0.0-alpha2'
}

Styles
 <style name="AppTheme" parent="Theme.MaterialComponents.Light.NoActionBar">
        <item name="textInputStyle">@style/AppTheme.OutlineBox</item>
        <item name="android:editTextStyle">@style/AppTheme.EditText</item>
 </style>

 
<style name="AppTheme.OutlineBox" parent="Widget.MaterialComponents.TextInputLayout.OutlinedBox">
        <item name="boxCornerRadiusBottomStart">8dp</item>
        <item name="boxCornerRadiusBottomEnd">8dp</item>
        <item name="boxCornerRadiusTopStart">8dp</item>
        <item name="boxCornerRadiusTopEnd">8dp</item>
        <item name="boxStrokeColor">@color/colorSecondary</item>-->
        <item name="hintTextAppearance">@style/AppTheme.OutlineBox.Hint</item>-->
</style>

<style name="AppTheme.OutlineBox.Hint">
        <item name="android:textColor">@color/colorSecondary</item>
        <item name="android:textSize">16sp</item>
</style>

<style name="AppTheme.EditText" parent="Widget.MaterialComponents.TextInputEditText.FilledBox">

</style>


XML Layout
<com.google.android.material.textfield.TextInputLayout
    android:id="@+id/textfield_layout"
    android:layout_width="match_parent"
    android:layout_height="wrap_content">
    <com.google.android.material.textfield.TextInputEditText
        android:id="@+id/textfield"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="@string/hint"
        android:imeOptions="actionNext"
        android:inputType="text"
        android:maxLines="1"
        android:singleLine="true"/>
</com.google.android.material.textfield.TextInputLayout>