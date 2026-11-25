---
title: "PivotCache.SourceCellArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotCache. Restituisce l'intervallo dell'origine dati utilizzato con SourceSheet"
type: docs
url: /it/net/aspose.cells.gridweb.data/pivotcache/sourcecellarea/
---
## PivotCache.SourceCellArea property

Restituisce l'intervallo dell'origine dati utilizzando SourceSheet.

```csharp
public WebCellArea SourceCellArea { get; }
```

### Esempi

```csharp

 [C#]

 //Modifica l'intervallo dell'origine dati
 //Valore originale: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 PivotTable table = GridWeb1.WebWorksheets.PivotTables["myPivotTable"];
 //Aggiunge dati di 2 righe
 table.PivotCache.SourceCellArea.EndRow = 12;

 [VB]

 'Changes data source range
 'Original value: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 Dim table As PivotTable =  GridWeb1.WebWorksheets.PivotTables("myPivotTable")
  'Adds 2 row data
 table.PivotCache.SourceCellArea.EndRow = 12
```

### Vedi anche

* class [WebCellArea](../../webcellarea/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


