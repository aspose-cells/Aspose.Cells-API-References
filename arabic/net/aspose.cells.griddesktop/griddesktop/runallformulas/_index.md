---
title: "GridDesktop.RunAllFormulas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "GridDesktop طريقة. ينفذ جميع صيغ الخلايا"
type: docs
url: /ar/net/aspose.cells.griddesktop/griddesktop/runallformulas/
---
## GridDesktop.RunAllFormulas method

ينفّذ جميع صيغ الخلايا.

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

### انظر أيضًا

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


