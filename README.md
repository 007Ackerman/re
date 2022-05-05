 <?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity2">

    <androidx.appcompat.widget.AppCompatImageView
        android:layout_width="@dimen/_22sdp"
        android:layout_height="@dimen/_22sdp"
        android:id="@+id/imagecategory"
        android:layout_marginStart="@dimen/_16sdp"
        android:layout_marginTop="@dimen/_16sdp"
        android:src="@drawable/ic_category"
        android:tint="@color/primary_label"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"/>


    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:id="@+id/textcategory"
        android:layout_marginStart="@dimen/_8sdp"
        android:text="Science Fiction"
        android:textColor="@color/primary_label"
        android:textSize="@dimen/_14ssp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="@id/imagecategory"
        app:layout_constraintStart_toEndOf="@id/imagecategory"
        app:layout_constraintTop_toTopOf="@id/imagecategory"/>

    <androidx.appcompat.widget.AppCompatImageView
        android:layout_width="@dimen/_22sdp"
        android:layout_height="@dimen/_22sdp"
        android:layout_marginStart="@dimen/_8sdp"
        android:tint="@color/primary_label"
        android:src="@drawable/ic_arrow_down"
        app:layout_constraintBottom_toBottomOf="@id/textcategory"
        app:layout_constraintStart_toEndOf="@id/textcategory"
        app:layout_constraintTop_toTopOf="@id/textcategory"/>

    <androidx.appcompat.widget.AppCompatImageView
        android:layout_width="@dimen/_22sdp"
        android:layout_height="@dimen/_22sdp"
        android:layout_marginTop="@dimen/_16sdp"
        android:layout_marginEnd="@dimen/_16sdp"
        android:src="@drawable/ic_notifications"
        android:tint="@color/secondaryy_label"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent"/>


    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:id="@+id/layoutsearch"
        android:layout_marginStart="@dimen/_16sdp"
        android:layout_marginTop="@dimen/_16sdp"
        android:layout_marginEnd="@dimen/_16sdp"
        android:background="@drawable/background_search"
        android:gravity="center_vertical"
        android:orientation="horizontal"
        android:paddingStart="@dimen/_16sdp"
        android:paddingEnd="@dimen/_16sdp"
        android:paddingTop="@dimen/_8sdp"
        android:paddingBottom="@dimen/_8sdp"
        app:layout_constraintTop_toBottomOf="@id/imagecategory">

        <androidx.appcompat.widget.AppCompatImageView
            android:layout_width="@dimen/_22sdp"
            android:layout_height="@dimen/_22sdp"
            android:src="@drawable/ic_search"
            android:tint="@color/primary_label"/>

        <EditText
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_marginStart="@dimen/_8sdp"
            android:background="@null"
            android:hint="Search"
            android:importantForAutofill="no"
            android:inputType="text"
            android:textColor="@color/primary_label"
            android:textColorHint="@color/secondaryy_label"
            android:textSize="@dimen/_13ssp"
            />

    </LinearLayout>

    <androidx.cardview.widget.CardView
        android:layout_width="match_parent"
        android:id="@+id/card"
        android:layout_height="wrap_content"
        android:layout_marginStart="@dimen/_30sdp"
        android:layout_marginEnd="@dimen/_30sdp"
        android:layout_marginBottom="@dimen/_16sdp"
        android:clickable="true"
        android:focusable="true"
        android:foreground="?android:attr/selectableItemBackground"
        app:cardCornerRadius="@dimen/_8sdp"
        app:cardElevation="@dimen/_3sdp"
        app:layout_constraintBottom_toTopOf="@id/smoothbottombar">




    <androidx.constraintlayout.widget.ConstraintLayout
        android:layout_width="match_parent"

        android:layout_height="wrap_content"
        android:padding="@dimen/_8sdp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent">

        <de.hdodenhof.circleimageview.CircleImageView
            android:id="@+id/healthimage"
            android:layout_width="@dimen/_80sdp"
            android:layout_height="@dimen/_80sdp"
            android:scaleType="centerCrop"
            android:src="@drawable/health"
            app:layout_constraintBottom_toBottomOf="parent"
            app:layout_constraintStart_toStartOf="parent"
            app:layout_constraintTop_toTopOf="parent" />

        <LinearLayout
            android:layout_width="207dp"
            android:layout_height="92dp"
            android:layout_marginTop="@dimen/_10sdp"
            android:layout_marginStart="@dimen/_10sdp"
            android:orientation="vertical"
            android:padding="@dimen/_8sdp"
            app:layout_constraintBottom_toBottomOf="parent"
            app:layout_constraintEnd_toEndOf="parent"
            app:layout_constraintStart_toEndOf="@id/healthimage"
            app:layout_constraintTop_toTopOf="parent">

            <TextView
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:ellipsize="end"
                android:maxLines="1"
                android:text="Healthcare Sector"
                android:textColor="@color/primary_label"
                android:textSize="@dimen/_12ssp"
                android:textStyle="bold" />

            <TextView
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginTop="@dimen/_3sdp"
                android:text="Healthcare Sector"
                android:textColor="@color/secondaryy_label"
                android:textSize="@dimen/_11ssp" />

            <TextView
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginTop="@dimen/_3sdp"
                android:text="Healthcare"
                android:textColor="@color/secondaryy_label"
                android:textSize="@dimen/_10ssp" />


        </LinearLayout>

        <androidx.appcompat.widget.AppCompatImageView
            android:layout_width="@dimen/_20sdp"
            android:layout_height="@dimen/_20sdp"
            android:background="@drawable/background_favourite"
            android:padding="@dimen/_5sdp"
            android:src="@drawable/ic_favorite"
            android:tint="@color/white"
            app:layout_constraintBottom_toBottomOf="parent"
            app:layout_constraintEnd_toEndOf="parent"/>



    </androidx.constraintlayout.widget.ConstraintLayout>

    </androidx.cardview.widget.CardView>

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:id="@+id/TextGraphs"
        android:layout_marginStart="@dimen/_16sdp"
        android:layout_marginBottom="@dimen/_20sdp"
        android:text="Graphs"
        android:textColor="@color/primary_label"
        android:textSize="@dimen/_13ssp"
        android:textStyle="bold"
        app:layout_constraintBottom_toTopOf="@id/card"
        app:layout_constraintStart_toStartOf="parent"/>

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginEnd="@dimen/_16sdp"
        android:text="View All"
        android:textColor="@color/secondaryy_label"
        android:textSize="@dimen/_11ssp"
        app:layout_constraintBottom_toBottomOf="@id/TextGraphs"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="@id/TextGraphs"/>

    <androidx.viewpager2.widget.ViewPager2
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:id="@+id/graphviewpage"
        android:layout_marginTop="@dimen/_24sdp"
        android:layout_marginBottom="@dimen/_24sdp"
        android:paddingStart="@dimen/_50sdp"
        android:paddingEnd="@dimen/_50sdp"
        app:layout_constraintBottom_toTopOf="@id/TextGraphs"
        app:layout_constraintTop_toBottomOf="@id/layoutsearch"/>



    <me.ibrahimsn.lib.SmoothBottomBar
        android:layout_width="match_parent"
        android:layout_height="@dimen/_60sdp"
        android:id="@+id/smoothbottombar"
        android:layout_marginStart="@dimen/_8sdp"
        android:layout_marginEnd="@dimen/_8sdp"
        android:layout_marginBottom="@dimen/_8sdp"
        android:background="@color/background"
        app:iconSize="@dimen/_18sdp"
        app:iconTint="@color/bottom_bar_icon"
        app:iconTintActive="@color/bottom_bar_icon_active"
        app:indicatorColor="@color/bottom_bar_indicator"
        app:indicatorRadius="@dimen/_80sdp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:menu="@menu/bottom_menu"
        app:textColor="@color/bottom_bar_text_color"
        app:textSize="@dimen/_10ssp"
        />

</androidx.constraintlayout.widget.ConstraintLayout>
