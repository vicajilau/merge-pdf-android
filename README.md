# merge-pdf-android

## 📄 Description

`merge-pdf-android` is a Kotlin library for Android that enables developers to merge multiple PDF files into a single document. It is designed to be lightweight, efficient, and easy to integrate into any Android project.

## ⚙️ Installation

Add the following to your `build.gradle` file:

```kotlin
dependencies {
    implementation("com.victorcarreras:merge-pdf-android:1.0.0")
}
```

## 🚀 Usage

Here’s a basic example of how to use the library:

```kotlin
val merger = PdfMerger(context)
val pdfList = listOf(file1, file2, file3) // List of File or Uri
val output = File(context.cacheDir, "merged.pdf")

merger.merge(pdfList, output) { success ->
    if (success) {
        // Handle success
    } else {
        // Handle failure
    }
}
```

## 🤝 Contributing
Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch (git checkout -b feature/your-feature-name).
3. Commit your changes (git commit -am 'Add new feature').
4. Push to the branch (git push origin feature/your-feature-name).
5. Open a Pull Request.