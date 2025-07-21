# 💾 SwiftUI Snippet Vault

Quick copy-paste helpers and patterns I reach for often.

---

### ✅ Dismiss a Sheet

```swift
@Environment(\.dismiss) var dismiss

Button("Done") {
  dismiss()
}
```
