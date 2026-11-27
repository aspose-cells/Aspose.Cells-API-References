---
title: "GridCell.GetFontColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCell-metod. Hämtar cellens teckensnittsfärg. När du ändrar färgen bör du anropa SetFontColor-metoden för att sätta teckensnittsfärgen på cellen"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridcell/getfontcolor/
---
## GridCell.GetFontColor method

Hämtar cellens teckensnittsfärg. När du ändrar färgen bör du anropa metoden "SetFontColor" för att sätta teckensnittsfärgen i cellen.

```csharp
public Color GetFontColor()
```

### Returvärde

returnera cellens teckensnittsfärg.

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


