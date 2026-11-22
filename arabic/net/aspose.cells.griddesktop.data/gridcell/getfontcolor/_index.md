---
title: "GridCell.GetFontColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridCell. يحصل على لون خط الخلية. عند تغيير اللون يجب استدعاء طريقة SetFontColor لتعيين لون الخط للخلية"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridcell/getfontcolor/
---
## GridCell.GetFontColor method

يحصل على لون خط الخلية. عند تغيير اللون، يجب استدعاء طريقة "SetFontColor" لتعيين لون الخط للخلية.

```csharp
public Color GetFontColor()
```

### قيمة الإرجاع

إرجاع لون خط الخلية.

### أمثلة

```csharp
[C#]
GridCell cell = gridDesktop1.GetActiveWorksheet().Cells[0, 0];
Font font = new Font("Courier New", 8, FontStyle.Italic);
cell.SetFont(font);
Color color = cell.GetFontColor();
color = Color.Black;
cell.SetFontColor(color);

[Visual Basic]
Dim cell As GridCell =  gridDesktop1.GetActiveWorksheet().Cells(0, 0) 
Dim font As Font =  New Font("Courier New",8,FontStyle.Italic) 
cell.SetFont(font)
Dim color As Color =  cell.GetFontColor() 
color = Color.Black
cell.SetFontColor(color)

```

### انظر أيضًا

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


