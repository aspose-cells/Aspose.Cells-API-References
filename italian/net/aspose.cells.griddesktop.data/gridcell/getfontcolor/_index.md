---
title: "GridCell.GetFontColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GridCell metodo. Ottiene il colore del carattere della cella. Quando si cambia il colore, è necessario invocare il metodo SetFontColor per impostare il colore del carattere nella cella"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridcell/getfontcolor/
---
## GridCell.GetFontColor method

Ottiene il colore del font della cella. Quando si cambia il colore, è necessario invocare il metodo "SetFontColor" per impostare il colore del font nella cella.

```csharp
public Color GetFontColor()
```

### Valore di ritorno

restituisce il colore del carattere della cella.

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


