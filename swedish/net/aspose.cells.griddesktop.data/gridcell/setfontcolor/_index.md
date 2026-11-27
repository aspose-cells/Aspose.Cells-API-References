---
title: "GridCell.SetFontColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCell method. Sätter teckensnittsfärgen för cellen. För att förbättra prestanda implementera SetFontColor‑metoden inte implementera FontColor‑egenskapen"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridcell/setfontcolor/
---
## GridCell.SetFontColor method

Sätter teckensnittsfärgen i cellen. För att förbättra prestanda, implementera metoden "SetFontColor" och inte egenskapen "FontColor".

```csharp
public void SetFontColor(Color color)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| färg | Färg | teckensnittsfärg att sättas. |

### Exempel

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

### Se även

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


