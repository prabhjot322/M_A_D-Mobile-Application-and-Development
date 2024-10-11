# Develop a program to implement table layout to display calculator.
## Code
```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical">

    <!-- Heading Section -->
    <TextView
        android:layout_width="match_parent"
        android:layout_height="102dp"
        android:background="#4CAF50"
        android:text="Calculator"
        android:textColor="#000000"
        android:padding="15dp"
        android:textSize="35sp"
        android:textStyle="bold" />

    <!-- Display Section (Reduced size) -->
    <TextView
        android:id="@+id/display"
        android:layout_width="match_parent"
        android:layout_height="441dp"
        android:background="#FFFFFF"
        android:gravity="end|bottom"
        android:padding="16dp"
        android:text="0"
        android:textColor="#000000"
        android:textSize="40sp" />

    <!-- Table Layout for Keypad (Expanded to cover full bottom space) -->
    <TableLayout
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:layout_weight="1"
        android:shrinkColumns="*"
        android:stretchColumns="*">

        <!-- First Row -->
        <TableRow>

            <Button
                android:id="@+id/button_ac"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#757575"
                android:padding="20dp"
                android:text="AC"
                android:textColor="#FFFFFF"
                android:textSize="24sp" />

            <Button
                android:id="@+id/button_paren_open"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#757575"
                android:padding="20dp"
                android:text="("
                android:textColor="#FFFFFF"
                android:textSize="24sp" />

            <Button
                android:id="@+id/button_paren_close"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#757575"
                android:padding="20dp"
                android:text=")"
                android:textColor="#FFFFFF"
                android:textSize="24sp" />

            <Button
                android:id="@+id/button_percent"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#757575"
                android:padding="20dp"
                android:text="%"
                android:textColor="#FFFFFF"
                android:textSize="24sp" />
        </TableRow>

        <!-- Second Row -->
        <TableRow>

            <Button
                android:id="@+id/button_7"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#D3D3D3"
                android:padding="20dp"
                android:text="7"
                android:textSize="24sp" />

            <Button
                android:id="@+id/button_8"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#D3D3D3"
                android:padding="20dp"
                android:text="8"
                android:textSize="24sp" />

            <Button
                android:id="@+id/button_9"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#D3D3D3"
                android:padding="20dp"
                android:text="9"
                android:textSize="24sp" />

            <Button
                android:id="@+id/button_divide"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#757575"
                android:padding="20dp"
                android:text="/"
                android:textColor="#FFFFFF"
                android:textSize="24sp" />
        </TableRow>

        <!-- Third Row -->
        <TableRow>

            <Button
                android:id="@+id/button_4"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#D3D3D3"
                android:padding="20dp"
                android:text="4"
                android:textSize="24sp" />

            <Button
                android:id="@+id/button_5"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#D3D3D3"
                android:padding="20dp"
                android:text="5"
                android:textSize="24sp" />

            <Button
                android:id="@+id/button_6"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#D3D3D3"
                android:padding="20dp"
                android:text="6"
                android:textSize="24sp" />

            <Button
                android:id="@+id/button_multiply"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#757575"
                android:padding="20dp"
                android:text="*"
                android:textColor="#FFFFFF"
                android:textSize="24sp" />
        </TableRow>

        <!-- Fourth Row -->
        <TableRow>

            <Button
                android:id="@+id/button_1"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#D3D3D3"
                android:padding="20dp"
                android:text="1"
                android:textSize="24sp" />

            <Button
                android:id="@+id/button_2"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#D3D3D3"
                android:padding="20dp"
                android:text="2"
                android:textSize="24sp" />

            <Button
                android:id="@+id/button_3"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#D3D3D3"
                android:padding="20dp"
                android:text="3"
                android:textSize="24sp" />

            <Button
                android:id="@+id/button_subtract"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#757575"
                android:padding="20dp"
                android:text="-"
                android:textColor="#FFFFFF"
                android:textSize="24sp" />
        </TableRow>

        <!-- Fifth Row -->
        <TableRow>

            <Button
                android:id="@+id/button_dot"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#D3D3D3"
                android:padding="20dp"
                android:text="."
                android:textSize="24sp" />

            <Button
                android:id="@+id/button_0"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#D3D3D3"
                android:padding="20dp"
                android:text="0"
                android:textSize="24sp" />

            <Button
                android:id="@+id/button_equals"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#FF5722"
                android:padding="20dp"
                android:text="="
                android:textColor="#FFFFFF"
                android:textSize="24sp" />

            <Button
                android:id="@+id/button_add"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:background="#757575"
                android:padding="20dp"
                android:text="+"
                android:textColor="#FFFFFF"
                android:textSize="24sp" />
        </TableRow>

    </TableLayout>

</LinearLayout>
```
## Output 
![WhatsApp Image 2024-09-29 at 12 06 12_111125c1](https://github.com/user-attachments/assets/8d553f38-6f7a-4f79-9c3d-5404ccf62642)
