---
title: "GridCells.SetBorders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCells-metod. Ställer in kanter för ett cellområde"
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridcells/setborders/
---
## GridCells.SetBorders method

Ställer in kanter för ett cellintervall.

```csharp
public void SetBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, 
    SetBorderPosition position, WebBorderStyle borderStyle)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Det första radnumret i intervallet (nollbaserat). |
| firstColumn | Int32 | Det första kolumnnumret i intervallet (nollbaserat). |
| rowNumber | Int32 | Antalet rader. |
| columnNumber | Int32 | Antalet kolumner. |
| position | SetBorderPosition | Kantpositionen. |
| borderStyle | WebBorderStyle | Marginalstilen. |

### Exempel

```csharp
[C#]
  GridWeb GridWeb1 = new GridWeb();
  WebBorderStyle borderStyle1 = new WebBorderStyle();
 GridWeb1.WorkSheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1);

[VB]
	GridWeb1.WebWorksheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1)
```

### Se även

* enum [SetBorderPosition](../../../aspose.cells.gridweb/setborderposition/)
* class [WebBorderStyle](../../../aspose.cells.gridweb/webborderstyle/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


