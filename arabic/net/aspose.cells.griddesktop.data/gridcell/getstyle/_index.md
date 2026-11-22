---
title: "GridCell.GetStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridCell. يحصل على نمط الخلية. عند تغيير النمط يجب استدعاء طريقة SetStyle لتعيين النمط للخلية"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridcell/getstyle/
---
## GridCell.GetStyle method

يحصل على نمط الخلية. عند تغيير النمط، يجب استدعاء طريقة "SetStyle" لتعيين النمط للخلية.

```csharp
public Style GetStyle()
```

### قيمة الإرجاع

إرجاع نسخة من نمط الخلية.

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


