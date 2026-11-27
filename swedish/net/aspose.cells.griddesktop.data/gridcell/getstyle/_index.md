---
title: "GridCell.GetStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCell-metod. Hämtar cellstil. När du ändrar stilen bör du anropa SetStyle-metoden för att sätta stil på cellen"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridcell/getstyle/
---
## GridCell.GetStyle method

Hämtar cellens stil. När du ändrar stilen bör du anropa metoden "SetStyle" för att sätta stilen i cellen.

```csharp
public Style GetStyle()
```

### Returvärde

returnera en kopia av cellstilen.

### Exempel

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

### Se även

* class [Style](../../../aspose.cells.griddesktop/style/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


