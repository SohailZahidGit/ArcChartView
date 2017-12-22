# ArcChartViewDemo
You can use this library to draw Arc charts

and show your statistics or anything you want

or maybe get some ratings from user.



## 1 - Getting Started

By this instructions you can add this library and i will explain how use it.

<img src="http://ikhoshabi.com/ss/gif/ArcChartView.gif" width="300">



### Add Maven to your root build.gradle

First of all Add it in your root build.gradle at the end of repositories:

```
allprojects {
  repositories {
    ...
    maven { url 'https://jitpack.io' }
  }
}
```

### Add Dependency

Add the dependency to your app build.gradle file

```
dependencies
{
    compile 'com.github.imaNNeoFighT:ArcChartView:-SNAPSHOT'
}
```

And then sync your gradle and take a tea.


## 2 - About The View
You can simply use this View like other Views in android,
just add ``ArcChartView`` in your java code or xml.

## View Properties
you can use this properties for make everything you want,
and all of them is arbitary,and can change via xml or java code/

* `acv_lines_count`
  by this property you can specify lines count of chart (i mean arc lines), default value is `10`

* `acv_lines_space`
  by this property you can specify lines space (lines margin), default value is `4dp`
  
* `acv_lines_width`
  by this property you can specify lines width , default value is `6dp`

* `acv_sections_count`
  by this property you can specify sections count , default value is `8`

* `acv_sections_space`
  by this property you can specify sections space (sections margin) , default value is `4dp`

* `acv_mid_start_extra_offset`
  by this property you can specify center extra offest size, default value is `16dp`

* `acv_icon_size`
  by this property you can specify the icons size, default value is `32dp`




## 3 - Use in Code


### Sample 1

```
    <com.neo.arcchartview.ArcChartView
        android:id="@+id/arc_chart_view"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toTopOf="@+id/view_separator"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:acv_lines_count="10"
        app:acv_lines_width="6dp"
        app:acv_lines_space="4dp"
        app:acv_sections_count="8"
        app:acv_sections_space="2dp"
        app:acv_icon_size="32dp"
        app:acv_mid_start_extra_offset="12dp"
        />
```
you will see this output

<img src="http://ikhoshabi.com/ss/ArcChartView/sample1.png" width="300">
