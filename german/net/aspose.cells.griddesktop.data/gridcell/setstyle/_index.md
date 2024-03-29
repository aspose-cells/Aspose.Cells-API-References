---
title: SetStyle
second_title: Aspose.Cells für .NET-API-Referenz
description: Legt den Stil auf die Zelle fest. Um die Leistung zu verbessern implementieren Sie die Methode SetStyle implementieren Sie die Eigenschaft Style nicht.
type: docs
weight: 420
url: /de/net/aspose.cells.griddesktop.data/gridcell/setstyle/
---
## GridCell.SetStyle method

Legt den Stil auf die Zelle fest. Um die Leistung zu verbessern, implementieren Sie die Methode "SetStyle", implementieren Sie die Eigenschaft "Style" nicht.

```csharp
public void SetStyle(Style value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | Style | Stil einzustellen. |

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

* class [Style](../../../aspose.cells.griddesktop/style)
* class [GridCell](../../gridcell)
* namensraum [Aspose.Cells.GridDesktop.Data](../../gridcell)
* Montage [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
