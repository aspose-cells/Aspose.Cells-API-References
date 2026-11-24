---
title: "PivotCache.SourceCellArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotCache-Eigenschaft. Gibt den Bereich der Datenquelle zurück, der mit SourceSheet verwendet wird"
type: docs
url: /de/net/aspose.cells.gridweb.data/pivotcache/sourcecellarea/
---
## PivotCache.SourceCellArea property

Gibt den Bereich der Datenquelle zurück, der mit SourceSheet verwendet wird.

```csharp
public WebCellArea SourceCellArea { get; }
```

### Beispiele

```csharp

 [C#]

 //Ändert den Datenquellenbereich
 //Ursprünglicher Wert: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 PivotTable table = GridWeb1.WebWorksheets.PivotTables["myPivotTable"];
 //Fügt 2 Zeilen Daten hinzu
 table.PivotCache.SourceCellArea.EndRow = 12;

 [VB]

 'Changes data source range
 'Original value: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 Dim table As PivotTable =  GridWeb1.WebWorksheets.PivotTables("myPivotTable")
  'Adds 2 row data
 table.PivotCache.SourceCellArea.EndRow = 12
```

### Siehe auch

* class [WebCellArea](../../webcellarea/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


