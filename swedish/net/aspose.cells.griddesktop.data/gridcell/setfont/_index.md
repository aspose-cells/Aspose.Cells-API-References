---
title: "GridCell.SetFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCell metod. Sätter teckensnitt för cellen. För att förbättra prestanda implementera SetFont‑metoden, inte implementera Font‑egenskapen"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridcell/setfont/
---
## GridCell.SetFont method

Sätter teckensnittet i cellen. För att förbättra prestanda, implementera metoden "SetFont" och inte egenskapen "Font".

```csharp
public void SetFont(Font font)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| teckensnitt | Teckensnitt | teckensnitt som ska sättas. |

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


