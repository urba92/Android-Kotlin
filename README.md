# Android Kotlin

[A density of the screen](https://developer.android.com/reference/kotlin/androidx/compose/ui/unit/Density)
```Kotlin
val sizeInPx = with(LocalDensity.current) { 16.dp.toPx() }
```

  val configuration = LocalConfiguration.current

val screenHeight = configuration.screenHeightDp.dp
val screenWidth = configuration.screenWidthDp.dp

Device orientation
```Kotlin
val configuration = LocalConfiguration.current
when (configuration.orientation) {
    Configuration.ORIENTATION_LANDSCAPE -> {
        Text("Landscape")
    }
    else -> {
        Text("Portrait")
    }
}
```
