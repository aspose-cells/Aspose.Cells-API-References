---
title: "PivotCache.SourceCellArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotCache egenskap. Returnerar intervallet för datakällan som används med SourceSheet"
type: docs
url: /sv/net/aspose.cells.gridweb.data/pivotcache/sourcecellarea/
---
## PivotCache.SourceCellArea property

Returnerar intervallet för datakällan som används med SourceSheet.

```csharp
public WebCellArea SourceCellArea { get; }
```

### Exempel

```csharp

 [C#]

 //Ändrar datakällans intervall
 //Ursprungligt värde: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 PivotTable table = GridWeb1.WebWorksheets.PivotTables["myPivotTable"];
 //Lägger till 2 rader data
 table.PivotCache.SourceCellArea.EndRow = 12;

 [VB]

 'Changes data source range
 'Original value: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 Dim table As PivotTable =  GridWeb1.WebWorksheets.PivotTables("myPivotTable")
  'Adds 2 row data
 table.PivotCache.SourceCellArea.EndRow = 12
```

### Se även

* class [WebCellArea](../../webcellarea/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


