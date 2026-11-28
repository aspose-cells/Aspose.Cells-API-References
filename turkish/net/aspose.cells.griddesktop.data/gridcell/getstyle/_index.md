---
title: "GridCell.GetStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridCell yöntemi. Hücre stilini alır. Stili değiştirdiğinizde, hücreye stili ayarlamak için SetStyle yöntemini çağırmalısınız."
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridcell/getstyle/
---
## GridCell.GetStyle method

Hücre stilini alır. Stili değiştirdiğinizde, hücreye stili ayarlamak için "SetStyle" metodunu çağırmalısınız.

```csharp
public Style GetStyle()
```

### Dönüş Değeri

hücre stilinin bir kopyasını döndür.

### Örnekler

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

### Ayrıca Bakınız

* class [Style](../../../aspose.cells.griddesktop/style/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


