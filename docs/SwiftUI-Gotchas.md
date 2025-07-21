# 🧠 SwiftUI Gotchas

A growing list of confusing behaviors, unexpected bugs, or “why is this like this” moments — and how to deal with them.

| Gotcha                                                   | Fix / Workaround                                               | Notes                        |
| -------------------------------------------------------- | -------------------------------------------------------------- | ---------------------------- |
| `.navigationBarHidden(true)` disables back swipe gesture | Use `.toolbar(.hidden)` instead                                | iOS 16+                      |
| `@State` not updating UI                                 | Use `@ObservedObject` or `@StateObject` if shared across views | Happens in tab views & forms |
| Preview not updating after Core Data changes             | Restart preview or delete derived data                         | Classic Xcode issue          |
| `.sheet()` doesn’t dismiss programmatically              | Use `@Environment(\.dismiss)`                                  | Works in iOS 15+             |
