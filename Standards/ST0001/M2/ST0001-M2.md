# 📌 Lyxbux Versioning (ST0001-M2)
**ST0001-M1** is not deprecated or broken — this document is an add-on that introduces additional recommendations, specifically for **MSBuild version properties**.

MSBuild supports semantic versioning using the format: `Major.Minor.Patch.Build`. This update encourages all future project releases to explicitly include version metadata in their `.csproj` files.

## 🔍 Why was this modification introduced?
Some developers have already released projects using **ST0001-M1**. Since they cannot modify existing published releases, this new recommendation helps them adopt proper versioning starting from their next release.

## ✅ Required Additions (to every .csproj file)
Add the following properties manually in each `.csproj`:

```xml
<FileVersion>1.0.0.0</FileVersion>
<AssemblyVersion>1.0.0.0</AssemblyVersion>
<InformationalVersion>1.0.0.0</InformationalVersion>
<IncludeSourceRevisionInInformationalVersion>false</IncludeSourceRevisionInInformationalVersion>
```

## 🔁 Semantic Version Mapping
As previously outlined in **ST0001-M1**, you can map your version identifiers like this:
- M1 → 1.0.0.0
- M2 → 2.0.0.0
- Mn → n.0.0.0