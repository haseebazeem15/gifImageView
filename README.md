[![](https://jitpack.io/v/haseebazeem15/gifImageView.svg)](https://jitpack.io/#haseebazeem15/gifImageView)
# GifImageView
GifImageView is light weight and efficient library to display Gif images in android application.


## Demo
![alt text](https://github.com/haseebazeem15/gifImageView/blob/master/ezgif-3-3a03e164f61a.gif)

## Minimum API LEVEL
GifImageView is compatible with API LEVEL 21 or above.

## Installation

1) Use [jitpack](https://jitpack.io) in your build.gradle file to install GifImageView.

```bash
allprojects {
 repositories {
   maven { url 'https://jitpack.io' }
 }
}
```
## Gradle
```bash
dependencies {
 implementation 'com.github.haseebazeem15:gifImageView:1.4'
}
```

## Usage

Create this GifImageView element in your layout xml file:

```java
<com.haseebazeem.sampleGif.GifImageView
   android:id="@+id/gifImage"
   android:layout_width="wrap_content"
   android:layout_height="wrap_content"
   app:src="@drawable/your_gif_file"
/>
```
Inflate GIF Drawable programmatically using:
```java

GifImageView gifImageView;

gifImageView = (GifImageView) findViewById(R.id.gifImage);
gifImageView.setGifImageResource(R.drawable.splashscreen);
```

Inflate GIF Uri using:
```java

GifImageView gifImageView;

gifImageView = (GifImageView) findViewById(R.id.gifImage);
Uri uri = URI_OF_YOUR_GIF_FILE
gifImageView.setGifImageUri(uri);
```

Inflate GIF using File object & Path:
```java

GifImageView gifImageView;

gifImageView = (GifImageView) findViewById(R.id.gifImage);
File file = new File("path/to/gif_file");
gifImageView.setGifImageFile(file);

String path = "path/to/gif_file";
gifImageView.setGifImageFile(path);
```

## Drawable Requirements
Make sure to import gif file in all drawable directories like drawable-v24, drawable etc.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
