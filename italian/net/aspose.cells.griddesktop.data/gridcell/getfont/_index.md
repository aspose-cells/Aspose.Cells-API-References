---
title: "GridCell.GetFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridCell. Restituisce il font della cella. Quando cambi il font, dovresti invocare il metodo SetFont per impostare il font sulla cella"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridcell/getfont/
---
## GridCell.GetFont method

Ottiene il font della cella. Quando si cambia il font, è necessario invocare il metodo "SetFont" per impostare il font nella cella.

```csharp
public Font GetFont()
```

### Valore di ritorno

Restituisce una copia del font della cella.

### Esempi

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

### Vedi anche

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


