---
title: "PivotCache.SourceCellArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotCache. Возвращает диапазон источника данных, используемый с SourceSheet"
type: docs
url: /ru/net/aspose.cells.gridweb.data/pivotcache/sourcecellarea/
---
## PivotCache.SourceCellArea property

Возвращает диапазон источника данных, используемый с SourceSheet.

```csharp
public WebCellArea SourceCellArea { get; }
```

### Примеры

```csharp

 [C#]

 //Изменяет диапазон источника данных
 //Исходное значение: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 PivotTable table = GridWeb1.WebWorksheets.PivotTables["myPivotTable"];
 //Добавляет данные 2 строк
 table.PivotCache.SourceCellArea.EndRow = 12;

 [VB]

 'Changes data source range
 'Original value: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 Dim table As PivotTable =  GridWeb1.WebWorksheets.PivotTables("myPivotTable")
  'Adds 2 row data
 table.PivotCache.SourceCellArea.EndRow = 12
```

### См. также

* class [WebCellArea](../../webcellarea/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


