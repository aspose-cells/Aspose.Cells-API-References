---
title: "GridCell.GetFontColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridCell yöntemi. Hücre yazı tipinin rengini alır. Rengi değiştirdiğinizde, hücreye yazı tipi rengi ayarlamak için SetFontColor yöntemini çağırmalısınız."
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridcell/getfontcolor/
---
## GridCell.GetFontColor method

Hücre yazı tipi rengini alır. Rengi değiştirdiğinizde, hücreye yazı tipi rengini ayarlamak için "SetFontColor" metodunu çağırmalısınız.

```csharp
public Color GetFontColor()
```

### Dönüş Değeri

hücre yazı tipi rengini döndür.

### Örnekler

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

### Ayrıca Bakınız

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


