---
title: "GridCell.GetFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCell-metod. Hämtar cellens teckensnitt. När du ändrar teckensnittet bör du anropa SetFont-metoden för att sätta teckensnittet på cellen"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridcell/getfont/
---
## GridCell.GetFont method

Hämtar cellens teckensnitt. När du ändrar teckensnittet bör du anropa metoden "SetFont" för att sätta teckensnittet i cellen.

```csharp
public Font GetFont()
```

### Returvärde

returnera en kopia av cellens teckensnitt.

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


