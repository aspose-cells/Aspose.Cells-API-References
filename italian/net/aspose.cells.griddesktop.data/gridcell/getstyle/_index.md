---
title: "GridCell.GetStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridCell. Restituisce lo stile della cella. Quando modifichi lo stile, dovresti invocare il metodo SetStyle per impostare lo stile sulla cella"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridcell/getstyle/
---
## GridCell.GetStyle method

Ottiene lo stile della cella. Quando si cambia lo stile, è necessario invocare il metodo "SetStyle" per impostare lo stile nella cella.

```csharp
public Style GetStyle()
```

### Valore di ritorno

Restituisce una copia dello stile della cella.

### Esempi

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

### Vedi anche

* class [Style](../../../aspose.cells.griddesktop/style/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


