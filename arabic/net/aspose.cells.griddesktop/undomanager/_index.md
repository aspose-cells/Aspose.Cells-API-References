---
title: "الفئة UndoManager"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridDesktop.UndoManager. تغلف الكائن الذي يدير عمليات التراجع/الإعادة"
type: docs
url: /ar/net/aspose.cells.griddesktop/undomanager/
---
## UndoManager class

يغلف الكائن الذي يدير عمليات التراجع/الإعادة.

```csharp
public class UndoManager
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Enabled](../../aspose.cells.griddesktop/undomanager/enabled/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كانت وظيفة التراجع مفعلة. القيمة الافتراضية هي false. |
| [RedoStepsCount](../../aspose.cells.griddesktop/undomanager/redostepscount/) { get; } | يحصل على عدد خطوات الإعادة المتاحة حاليًا. |
| [UndoStackSize](../../aspose.cells.griddesktop/undomanager/undostacksize/) { get; set; } | يحصل أو يضبط حجم مكدس التراجع/الإعادة. القيمة الافتراضية هي 300. |
| [UndoStepsCount](../../aspose.cells.griddesktop/undomanager/undostepscount/) { get; } | يحصل على عدد خطوات التراجع المتاحة حاليًا. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [BeginChanges](../../aspose.cells.griddesktop/undomanager/beginchanges/)() | يبدأ في تسجيل التغييرات. |
| [BeginMark](../../aspose.cells.griddesktop/undomanager/beginmark/)() | يبدأ في وضع علامة على التغييرات. |
| [ClearStack](../../aspose.cells.griddesktop/undomanager/clearstack/)() | يمسح مكدسات التراجع والإعادة. |
| [EndChanges](../../aspose.cells.griddesktop/undomanager/endchanges/)() | ينتهي من تسجيل التغييرات. |
| [EndMark](../../aspose.cells.griddesktop/undomanager/endmark/)() | ينتهي من وضع علامة على التغييرات. |
| [Redo](../../aspose.cells.griddesktop/undomanager/redo/)() | ينفذ عملية إعادة. |
| [RedoMark](../../aspose.cells.griddesktop/undomanager/redomark/)() | ينفذ عملية إعادة مع علامة. |
| [Undo](../../aspose.cells.griddesktop/undomanager/undo/)() | ينفذ عملية تراجع. |
| [UndoMark](../../aspose.cells.griddesktop/undomanager/undomark/)() | ينفذ عملية تراجع مع علامة. |

### انظر أيضًا

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


