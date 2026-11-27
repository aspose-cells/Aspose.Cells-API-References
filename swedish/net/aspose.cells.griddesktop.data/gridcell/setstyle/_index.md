---
title: "GridCell.SetStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCell method. Sätter stil för cellen. För att förbättra prestanda implementera SetStyle‑metoden inte implementera Style‑egenskapen"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridcell/setstyle/
---
## GridCell.SetStyle method

Ställer in stil för cellen. För att förbättra prestanda, implementera "SetStyle"-metoden, inte implementera "Style"-egenskapen.

```csharp
public void SetStyle(Style value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | stil att sättas. |

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


