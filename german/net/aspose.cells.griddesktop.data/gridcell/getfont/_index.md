---
title: "GridCell.GetFont"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridCell-Methode. Gibt die Zellen-Schriftart zurück. Wenn die Schriftart geändert wird, sollten Sie die SetFont-Methode aufrufen, um die Schriftart für die Zelle festzulegen."
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridcell/getfont/
---
## GridCell.GetFont method

Liest die Zellen­schriftart. Wenn die Schriftart geändert wird, sollten Sie die Methode "SetFont" aufrufen, um die Schriftart für die Zelle festzulegen.

```csharp
public Font GetFont()
```

### Rückgabewert

Gibt eine Kopie der Zellen-Schriftart zurück.

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


