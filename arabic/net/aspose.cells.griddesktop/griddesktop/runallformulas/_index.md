---
title: RunAllFormulas
second_title: Aspose.Cells لمرجع .NET API
description: يقوم بتشغيل صيغة كل الخلايا.
type: docs
weight: 770
url: /ar/net/aspose.cells.griddesktop/griddesktop/runallformulas/
---
## GridDesktop.RunAllFormulas method

يقوم بتشغيل صيغة كل الخلايا.

```csharp
public void RunAllFormulas()
```

### أمثلة

```csharp
[C#]
gridDesktop1.Worksheets[0].Cells[0, 0].Value = "2";
gridDesktop1.Worksheets[0].Cells[1, 0].Value = "3";
gridDesktop1.Worksheets[0].Cells[2, 1].Value = "=a1*a2";
gridDesktop1.RunAllFormulas();
gridDesktop1.Invalidate();

[Visual Basic]
gridDesktop1.Worksheets(0).Cells(0, 0).Value = "2"
gridDesktop1.Worksheets(0).Cells(1, 0).Value = "3"
gridDesktop1.Worksheets(0).Cells(2, 1).Value = "=a1*a2"
gridDesktop1.RunAllFormulas()
gridDesktop1.Invalidate()

```

### أنظر أيضا

* class [GridDesktop](../../griddesktop)
* مساحة الاسم [Aspose.Cells.GridDesktop](../../griddesktop)
* المجسم [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
