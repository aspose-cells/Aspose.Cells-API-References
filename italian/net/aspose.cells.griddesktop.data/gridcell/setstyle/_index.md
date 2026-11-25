---
title: "GridCell.SetStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridCell. Imposta lo stile della cella. Per migliorare le prestazioni implementare il metodo SetStyle invece di implementare la proprietà Style"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridcell/setstyle/
---
## GridCell.SetStyle method

Imposta lo stile nella cella. Per migliorare le prestazioni, implementare il metodo "SetStyle", non implementare la proprietà "Style".

```csharp
public void SetStyle(Style value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | Stile | stile da impostare. |

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


