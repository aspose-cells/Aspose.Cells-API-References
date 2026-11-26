---
title: "PivotCache.SourceCellArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotCache. Devuelve el rango de la fuente de datos usando SourceSheet"
type: docs
url: /es/net/aspose.cells.gridweb.data/pivotcache/sourcecellarea/
---
## PivotCache.SourceCellArea property

Devuelve el rango de la fuente de datos usando SourceSheet.

```csharp
public WebCellArea SourceCellArea { get; }
```

### Ejemplos

```csharp

 [C#]

 //Cambia el rango de la fuente de datos
 //Valor original: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 PivotTable table = GridWeb1.WebWorksheets.PivotTables["myPivotTable"];
 //Agrega datos de 2 filas
 table.PivotCache.SourceCellArea.EndRow = 12;

 [VB]

 'Changes data source range
 'Original value: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 Dim table As PivotTable =  GridWeb1.WebWorksheets.PivotTables("myPivotTable")
  'Adds 2 row data
 table.PivotCache.SourceCellArea.EndRow = 12
```

### Ver también

* class [WebCellArea](../../webcellarea/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


