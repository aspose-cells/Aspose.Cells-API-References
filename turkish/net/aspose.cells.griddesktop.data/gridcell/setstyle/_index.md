---
title: "GridCell.SetStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridCell yöntemi. Hücreye stil ayarlar. Performansı artırmak için Style özelliğini uygulamak yerine SetStyle yöntemini uygulayın"
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridcell/setstyle/
---
## GridCell.SetStyle method

Hücreye stili ayarlar. Performansı artırmak için "SetStyle" yöntemini uygulayın, "Style" özelliğini uygulamayın.

```csharp
public void SetStyle(Style value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | Stil | ayarılacak stil. |

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


