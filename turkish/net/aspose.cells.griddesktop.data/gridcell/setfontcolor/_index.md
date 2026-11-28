---
title: "GridCell.SetFontColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridCell yöntemi. Yazı tipi rengini hücreye ayarlar. Performansı artırmak için SetFontColor yöntemini uygulayın, FontColor özelliğini uygulamayın"
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridcell/setfontcolor/
---
## GridCell.SetFontColor method

Hücreye yazı tipi rengini ayarlar. Performansı artırmak için "SetFontColor" yöntemini uygulayın, "FontColor" özelliğini uygulamayın.

```csharp
public void SetFontColor(Color color)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color | Color | yazı tipi rengi ayarlanacak. |

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


