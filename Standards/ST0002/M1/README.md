# 📦 Uniplace

I'm currently not publishing binaries.
If you're using my libraries, you'll need to clone the repository and compile manually.
Sorry for the inconvenience — but this actually saves time during development ⏱️.

All compiled binaries are placed in a unified output folder:
📁 `C:\Publish`

To achieve this, I manually added the following to every `.csproj` file:

```xml
<AppendTargetFrameworkToOutputPath>false</AppendTargetFrameworkToOutputPath>
<AppendRuntimeIdentifierToOutputPath>false</AppendRuntimeIdentifierToOutputPath>
<OutputPath>C:\Publish</OutputPath>
```

This ensures that all your builds — from different libraries — drop their output into the same location, without extra subfolders.

## ⚠️ Warning
My projects are all created using **Visual Studio** with default build settings:
- 🔧 **Configuration:** `Debug`
- 💻 **Platform:** `Any CPU`

So make sure your build settings match, or adjust them as needed.

## ✅ Recommendation
- I recommend you apply the same `<OutputPath>` structure to your own FOSS projects.
- It helps keep things centralized, clean, and easy to manage — especially when working with multiple libraries.
- 💬 If you know of a better or more flexible setup, feel free to share it — so we can help other fellow FOSS developers benefit too!