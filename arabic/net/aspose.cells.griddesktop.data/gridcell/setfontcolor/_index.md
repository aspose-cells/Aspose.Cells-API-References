---
title: "GridCell.SetFontColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridCell. تعيين لون الخط للخلية. لتحسين الأداء تنفيذ طريقة SetFontColor بدلاً من تنفيذ خاصية FontColor"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridcell/setfontcolor/
---
## GridCell.SetFontColor method

يضبط لون الخط للخلية. لتحسين الأداء، نفّذ طريقة "SetFontColor"، لا تنفّذ خاصية "FontColor".

```csharp
public void SetFontColor(Color color)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اللون | اللون | لون الخط ليتم تعيينه. |

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


