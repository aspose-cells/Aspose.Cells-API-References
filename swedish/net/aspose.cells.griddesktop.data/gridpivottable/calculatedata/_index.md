---
title: "GridPivotTable.CalculateData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridPivotTable-metod. Beräknar pivottabellers data till cellerna"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridpivottable/calculatedata/
---
## GridPivotTable.CalculateData method

Beräknar pivottable:s data till celler.

```csharp
public void CalculateData()
```

### Anmärkningar

Cell.Value i pivotrangen kan inte returnera korrekt resultat om metoden inte har anropats. Denna metod beräknar data med en intern pivotcache, inte den ursprungliga datakällan. Så om datakällan har ändrats, vänligen anropa RefreshData()-metoden först.

### Se även

* class [GridPivotTable](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


