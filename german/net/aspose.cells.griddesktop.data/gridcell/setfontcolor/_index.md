---
title: "GridCell.SetFontColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridCell-Methode. Setzt die Schriftfarbe der Zelle. Zur Leistungsverbesserung SetFontColor-Methode implementieren, nicht die FontColor-Eigenschaft."
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridcell/setfontcolor/
---
## GridCell.SetFontColor method

Setzt die Schriftfarbe für die Zelle. Um die Leistung zu verbessern, implementieren Sie die Methode "SetFontColor", nicht die Eigenschaft "FontColor".

```csharp
public void SetFontColor(Color color)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Farbe | Farbe | Schriftfarbe, die gesetzt werden soll. |

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


