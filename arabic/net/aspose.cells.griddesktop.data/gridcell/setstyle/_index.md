---
title: "GridCell.SetStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridCell. تُعيّن النمط للخلية. لتحسين الأداء يُنصح بتنفيذ طريقة SetStyle بدلاً من تنفيذ خاصية Style"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridcell/setstyle/
---
## GridCell.SetStyle method

يضبط النمط للخلية. لتحسين الأداء، نفّذ طريقة "SetStyle"، لا تنفّذ خاصية "Style".

```csharp
public void SetStyle(Style value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | النمط | النمط الذي سيتم تعيينه. |

### أمثلة

```csharp
[C#]
Style style = sheet.GetCell(0, 0).GetStyle();
style.CellLocked = true;
style.VAlignment = VerticalAlignmentType.Top;
...
sheet.GetCell(0, 0).SetStyle(style);

[Visual Basic]
Dim style As Style =  sheet.GetCell(0,0).GetStyle() 
style.CellLocked = True
style.VAlignment = VerticalAlignmentType.Top
...
sheet.GetCell(0, 0).SetStyle(style)

```

### انظر أيضًا

* class [Style](../../../aspose.cells.griddesktop/style/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


