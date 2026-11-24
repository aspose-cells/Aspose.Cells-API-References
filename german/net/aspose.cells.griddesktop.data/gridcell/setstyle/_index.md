---
title: "GridCell.SetStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridCell-Methode. Setzt den Stil der Zelle. Zur Leistungsverbesserung SetStyle-Methode implementieren, nicht die Style-Eigenschaft."
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridcell/setstyle/
---
## GridCell.SetStyle method

Setzt den Stil für die Zelle. Um die Leistung zu verbessern, implementieren Sie die Methode "SetStyle", nicht die Eigenschaft "Style".

```csharp
public void SetStyle(Style value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | Stil | Stil, der gesetzt werden soll. |

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


