---
title: "GridCell.SetFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridCell. Imposta il carattere nella cella. Per migliorare le prestazioni implementare il metodo SetFont, non implementare la proprietà Font."
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridcell/setfont/
---
## GridCell.SetFont method

Imposta il carattere nella cella. Per migliorare le prestazioni, implementare il metodo "SetFont", non implementare la proprietà "Font".

```csharp
public void SetFont(Font font)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| font | Font | carattere da impostare. |

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


