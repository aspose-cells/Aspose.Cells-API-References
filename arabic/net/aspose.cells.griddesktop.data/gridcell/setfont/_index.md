---
title: SetFont
second_title: Aspose.Cells لمرجع .NET API
description: تعيين الخط على الخلية . لتحسين الأداء  قم بتنفيذ طريقة SetFont  لا تنفذ خاصية الخط .
type: docs
weight: 380
url: /ar/net/aspose.cells.griddesktop.data/gridcell/setfont/
---
## GridCell.SetFont method

تعيين الخط على الخلية . لتحسين الأداء ، قم بتنفيذ طريقة "SetFont" ، لا تنفذ خاصية "الخط" .

```csharp
public void SetFont(Font font)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| font | Font | سيتم تعيين الخط. |

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

### أنظر أيضا

* class [GridCell](../../gridcell)
* مساحة الاسم [Aspose.Cells.GridDesktop.Data](../../gridcell)
* المجسم [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
