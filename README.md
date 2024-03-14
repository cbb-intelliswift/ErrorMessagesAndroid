# ErrorMessagesAndroid
This is customise  android library to display Error, Message and Loading.

# How to use
1. Add it in your settings.graddle file
   
   dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
    repositories {
        google()
        mavenCentral()
        maven { url = uri("https://jitpack.io") }
    }
}

3. Import library from Maven Central repository:

   implementation("com.github.cbb-intelliswift:ErrorMessagesAndroid:1.1.1")
   
4. XML
   Here example of show error message

   <com.intelliswift.errormessagelib.ErrorMessages
        android:id="@+id/errorMsg"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_gravity="center"
        android:background="#DDD"
        android:clickable="true"
        android:focusable="true"
        android:visibility="gone"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toBottomOf="@id/btn_close" />

   5. Method you can use to show error message

      showMessage(...) // show suitable UI for a message
      showError(...) // show suitable UI for an error
      showInternetError(...) // show suitable UI for an Internet not found error
      showNoData(...) // show suitable UI for Data Not Available
      showLoading(...) // show suitable UI initializing loading

      Install
      https://www.jitpack.io/#cbb-intelliswift/ErrorMessagesAndroid/1.1.1
   
   

   

