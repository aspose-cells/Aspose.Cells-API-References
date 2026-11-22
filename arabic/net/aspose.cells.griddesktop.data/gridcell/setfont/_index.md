---
title: "GridCell.SetFont"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridCell. تعيين الخط للخلية. لتحسين الأداء تنفيذ طريقة SetFont بدلاً من تنفيذ خاصية Font"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridcell/setfont/
---
## GridCell.SetFont method

يضبط الخط للخلية. لتحسين الأداء، نفّذ طريقة "SetFont"، لا تنفّذ خاصية "Font".

```csharp
public void SetFont(Font font)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خط | خط | الخط ليتم تعيينه. |

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


