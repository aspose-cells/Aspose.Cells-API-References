---
title: "GridCell.GetFontColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridCell-Methode. Gibt die Zellen-Schriftfarbe zurück. Wenn die Farbe geändert wird, sollten Sie die SetFontColor-Methode aufrufen, um die Schriftfarbe für die Zelle festzulegen."
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridcell/getfontcolor/
---
## GridCell.GetFontColor method

Liest die Schriftfarbe der Zelle. Wenn die Farbe geändert wird, sollten Sie die Methode "SetFontColor" aufrufen, um die Schriftfarbe für die Zelle festzulegen.

```csharp
public Color GetFontColor()
```

### Rückgabewert

Gibt die Zellen-Schriftfarbe zurück.

### Beispiele

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

### Siehe auch

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


