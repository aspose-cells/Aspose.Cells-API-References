---
title: "GridCell.SetFont"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridCell yöntemi. Yazı tipini hücreye ayarlar. Performansı artırmak için SetFont yöntemini uygulayın, Font özelliğini uygulamayın"
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridcell/setfont/
---
## GridCell.SetFont method

Hücreye yazı tipini ayarlar. Performansı artırmak için "SetFont" yöntemini uygulayın, "Font" özelliğini uygulamayın.

```csharp
public void SetFont(Font font)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yazı tipi | Yazı Tipi | yazı tipi ayarlanacak. |

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


