grid-view-header
================

Take from http://grepcode.com/file/repository.grepcode.com/java/ext/com.google.android/android-apps/4.3_r2.1/com/android/photos/views/HeaderGridView.java

Usage:

Add HeaderGridView to layout:

    <com.cosic.gridviewheader.HeaderGridView
        android:id="@+id/grid_view_header"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        />

Programmically add header:

        View header = LayoutInflater.from(getContext()).inflate(R.layout.header, this, false);
        HeaderGridView grid = (HeaderGridView) findViewById(R.id.grid_view_header);
        grid.addHeaderView(header);
        grid.setAdapter(adapter);
