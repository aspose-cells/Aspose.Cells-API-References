---
title: "GridCell.SetFontColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridCell. Imposta il colore del carattere nella cella. Per migliorare le prestazioni implementare il metodo SetFontColor, non implementare la proprietà FontColor."
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridcell/setfontcolor/
---
## GridCell.SetFontColor method

Imposta il colore del carattere nella cella. Per migliorare le prestazioni, implementare il metodo "SetFontColor", non implementare la proprietà "FontColor".

```csharp
public void SetFontColor(Color color)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colore | Color | colore del carattere da impostare. |

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


