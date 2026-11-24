---
title: "GridCell.GetStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridCell Methode. Gibt den Zellenstil zurück. Wenn Sie den Stil ändern, sollten Sie die SetStyle‑Methode aufrufen, um den Stil der Zelle festzulegen"
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridcell/getstyle/
---
## GridCell.GetStyle method

Liest den Zellenstil. Wenn der Stil geändert wird, sollten Sie die Methode "SetStyle" aufrufen, um den Stil für die Zelle festzulegen.

```csharp
public Style GetStyle()
```

### Rückgabewert

Gibt eine Kopie des Zellenstils zurück.

### Beispiele

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

### Siehe auch

* class [Style](../../../aspose.cells.griddesktop/style/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


