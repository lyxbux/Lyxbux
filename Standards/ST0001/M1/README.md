# 📌 Lyxbux Versioning
I created a simple versioning system for my projects — designed to reduce confusion around major, minor, and patch disputes. This approach can work for individual developers or organizations who want a clean, stress-free way to version software.

## 🔢 How It Works
This versioning uses a single-part version called a modification, denoted by `M`.
- The format is `M1`, `M2`, `M3`, ..., increasing by `1` with every release.
- No patch/minor/major parts — just `M` + a number.

### 💡 Examples
- `M1`: Initial release (first public version)
- `M2`: Bug fix, small improvements
- `M3`: Major changes or new features

## 🎯 Why Use This?
Most users don't remember complex version numbers like `1.4.2`.
They just want to know: *Is it updated?*
This system makes it easy for both **users and developers** to reference versions without thinking in decimals.

## 🔁 Optional: Convert to Semantic
- If needed, you can easily convert this to a semantic format:
- Use `M` as the major version.
- Minor, patch, and build numbers can stay at `0`.
 - Example: `M5` becomes `5.0.0.0`.

## 📖 Where's the Detail?
The version number doesn't carry details about bug fixes or features.
Instead, that information belongs in your **changelog**, **commit history**, or **README**.