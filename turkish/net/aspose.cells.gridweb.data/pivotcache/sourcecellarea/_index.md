---
title: "PivotCache.SourceCellArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotCache özelliği. SourceSheet ile kullanılan veri kaynağının aralığını döndürür"
type: docs
url: /tr/net/aspose.cells.gridweb.data/pivotcache/sourcecellarea/
---
## PivotCache.SourceCellArea property

SourceSheet ile kullanılan veri kaynağının aralığını döndürür.

```csharp
public WebCellArea SourceCellArea { get; }
```

### Örnekler

```csharp

 [C#]

 //Veri kaynağı aralığını değiştirir
 //Orijinal değer: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 PivotTable table = GridWeb1.WebWorksheets.PivotTables["myPivotTable"];
 //2 satır veri ekler
 table.PivotCache.SourceCellArea.EndRow = 12;

 [VB]

 'Changes data source range
 'Original value: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 Dim table As PivotTable =  GridWeb1.WebWorksheets.PivotTables("myPivotTable")
  'Adds 2 row data
 table.PivotCache.SourceCellArea.EndRow = 12
```

### Ayrıca Bakınız

* class [WebCellArea](../../webcellarea/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


