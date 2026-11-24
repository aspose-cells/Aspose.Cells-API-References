---
title: "GridCell.SetFont"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridCell-Methode. Setzt die Schriftart für die Zelle. Um die Leistung zu verbessern, SetFont-Methode implementieren, nicht die Font-Eigenschaft"
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridcell/setfont/
---
## GridCell.SetFont method

Setzt die Schriftart für die Zelle. Um die Leistung zu verbessern, implementieren Sie die Methode "SetFont", nicht die Eigenschaft "Font".

```csharp
public void SetFont(Font font)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schriftart | Schriftart | zu setzende Schriftart. |

### Beispiele

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

### Siehe auch

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


