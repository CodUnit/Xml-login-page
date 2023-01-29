# Xml-login-page
 Xml Login Page using Linear Layout
<?xml version="1.0" encoding="utf-8"?>
<ScrollView xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:fitsSystemWindows="true">

    <LinearLayout
        android:orientation="vertical"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:paddingTop="56dp"
        android:paddingLeft="24dp"
        android:paddingRight="24dp">

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_marginBottom="24dp"
            android:textSize="24sp"
            android:text="PRODUCT LISTING"
            android:layout_gravity="center_horizontal" />

        (html comment removed:  Email Label )
        <android.support.design.widget.TextInputLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="8dp"
            android:layout_marginBottom="8dp">
            <EditText android:id="@+id/input_email"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:inputType="textEmailAddress"
                android:hint="Email" />
        </android.support.design.widget.TextInputLayout>

        (html comment removed:  Password Label )
        <android.support.design.widget.TextInputLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="8dp"
            android:layout_marginBottom="8dp">
            <EditText android:id="@+id/input_password"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:inputType="textPassword"
                android:hint="Password"/>
        </android.support.design.widget.TextInputLayout>

        <android.support.v7.widget.AppCompatButton
            android:id="@+id/btn_login"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="24dp"
            android:textColor="@color/colorWhite"
            android:layout_marginBottom="24dp"
            android:padding="12dp"
            android:text="Login"/>

        <TextView android:id="@+id/signup_text"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginBottom="24dp"
            android:text="Don't have an account? Sign Up"
            android:gravity="center"
            android:textSize="16dip"/>

    </LinearLayout>
</ScrollView>
The above xml describe that you have 2 Label, 2 TextInputLayout and 1 Login Button. When the user clicks the Login Button, it will redirect to the product listing page. It hasn’t validate if the user is valid or not. You can validate from your own needs.

And in the login there is signup option via text. So, we need to make our layout and its java class though. This is the signup layout xml file. I named it activity_signup.xml

<?xml version="1.0" encoding="utf-8"?>
<ScrollView
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:fitsSystemWindows="true">

    <LinearLayout
        android:orientation="vertical"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:paddingTop="56dp"
        android:paddingLeft="24dp"
        android:paddingRight="24dp">

        <TextView 
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textSize="24sp"
            android:text="@string/product_listing"
            android:layout_marginBottom="24dp"
            android:layout_gravity="center_horizontal" />

        (html comment removed:   Name Label )
        <android.support.design.widget.TextInputLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="8dp"
            android:layout_marginBottom="8dp">
            <EditText android:id="@+id/input_name"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:inputType="textCapWords"
                android:hint="@string/name" />
        </android.support.design.widget.TextInputLayout>

        (html comment removed:  Email Label )
        <android.support.design.widget.TextInputLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="8dp"
            android:layout_marginBottom="8dp">
            <EditText android:id="@+id/input_email"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:inputType="textEmailAddress"
                android:hint="@string/email" />
        </android.support.design.widget.TextInputLayout>

        (html comment removed:  Password Label )
        <android.support.design.widget.TextInputLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="8dp"
            android:layout_marginBottom="8dp">
            <EditText android:id="@+id/input_password"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:inputType="textPassword"
                android:hint="@string/password"/>
        </android.support.design.widget.TextInputLayout>

        (html comment removed:  Signup Button )
        <android.support.v7.widget.AppCompatButton
            android:id="@+id/btn_signup"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="24dp"
            android:layout_marginBottom="24dp"
            android:background="@color/colorPrimary"
            android:textColor="@color/colorWhite"
            android:padding="12dp"
            android:text="@string/create_account"/>

        <TextView android:id="@+id/login_text"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginBottom="24dp"
            android:text="@string/account_desc"
            android:gravity="center"
            android:textSize="16sp"/>

    </LinearLayout>
</ScrollView>
