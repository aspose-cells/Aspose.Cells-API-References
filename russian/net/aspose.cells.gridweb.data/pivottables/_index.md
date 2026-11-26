---
title: "Класс PivotTables"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.Data.PivotTables. Представляет коллекцию всех объектов PivotTable."
type: docs
url: /ru/net/aspose.cells.gridweb.data/pivottables/
---
## PivotTables class

Представляет коллекцию всех объектов [`PivotTable`](../pivottable/).

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotTables : ICollection
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivottables/count/) { get; } | Возвращает количество элементов, содержащихся в экземпляре PivotTables. |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivottables/issynchronized/) { get; } | Возвращает значение, указывающее, синхронизирован ли доступ к PivotTables (потокобезопасный). |
| [Item](../../aspose.cells.gridweb.data/pivottables/item/) { get; } | Получает объект PivotTable по индексу. (2 индексатора) |
| [Parent](../../aspose.cells.gridweb.data/pivottables/parent/) { get; } | Получает родительский объект для указанного объекта. Только для чтения. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivottables/syncroot/) { get; } | Получает объект, который можно использовать для синхронизации доступа к PivotTables. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add)(PivotCache) | Добавляет объект PivotTable из указанного PivotCache в новый лист. |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_3)(PivotCache, string) | Добавляет объект PivotTable из указанного PivotCache в новый лист. |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_1)(PivotCache, WebWorksheet, WebCell) | Добавляет объект PivotTable из указанного PivotCache в указанный лист. |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_2)(PivotCache, WebWorksheet, WebCell, string) | Добавляет объект PivotTable из указанного PivotCache в указанный лист. |
| [Clear](../../aspose.cells.gridweb.data/pivottables/clear/)() | Удаляет все объекты PivotTable и все объекты PivotCache в элементе управления. |
| [Contains](../../aspose.cells.gridweb.data/pivottables/contains/)(string) | Возвращает true, если существует PivotTable с именем tableName. |
| [CopyTo](../../aspose.cells.gridweb.data/pivottables/copyto/)(Array, int) | Копирует всю PivotTable в совместимый одномерный массив, начиная с указанного индекса целевого массива |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivottables/getenumerator/)() | Возвращает IEnumerator для PivotTables. |
| [Refresh](../../aspose.cells.gridweb.data/pivottables/refresh/)(PivotTable) | Повторно привязывает источник данных к отчету PivotTable. |
| [RefreshAll](../../aspose.cells.gridweb.data/pivottables/refreshall/)() | Повторно привязывает источник данных ко всем отчетам PivotTable. |
| [Remove](../../aspose.cells.gridweb.data/pivottables/remove/)(PivotTable) | Удаляет указанный объект PivotTable из PivotTables и связанный PivotCache, если он не используется другими PivotTable |
| [RemoveAt](../../aspose.cells.gridweb.data/pivottables/removeat/)(int) | Удаляет указанный объект PivotTable из PivotTables и связанный PivotCache, если он не используется другими PivotTable |

### Примечания

ПРИМЕЧАНИЕ: Этот класс теперь устарел. пожалуйста, используйте вместо него GridPivotTableCollection. Этот класс будет удалён через 6 месяцев после августа 2014 г. Aspose просит прощения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp

 [C#]

 //При предположении, что лист "Sheet1" содержит данные, создаётся отчёт PivotTable на его основе.
 WebWorksheet sourceSheet = GridWeb1.WebWorksheets["Sheet1"];
 Aspose.Cells.GridWeb.Data.WebCellArea sourceRange = new WebCellArea();
 sourceRange.StartRow = 0;
 sourceRange.StartColumn = 0;
 sourceRange.EndRow = 10;
 sourceRange.EndColumn = 5;

 PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(sourceSheet, sourceRange);

 PivotTable table = cache.CreatePivotTable();

 table.PivotFields[0].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[1].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[2].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[3].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;
 table.PivotFields[4].Orientation = PivotFieldOrientation.ColumnField;
 table.PivotFields[5].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;

 table.PivotFields[3].Function = PivotFieldFunction.Count;
 table.PivotFields[5].Function = PivotFieldFunction.Sum;

 table.DataBind();

 //Создаёт отчёт PivotTable из DataView или DataTable.
 DataView dataView;//Or  DataTable dataTable;
     .
     .
     .
 Sets dataView(dataTable) Value
     .
     .
     .

 PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataView);
 //Или PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataTable);
 PivotTable table = cache.CreatePivotTable();
 table = GridWeb1.WebWorksheets.PivotTables["PivotTable1"];
 table.PivotFields[0].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[1].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[2].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;
 table.DataBind();


 [VB]


 'On the assumption that worksheet "Sheet1" has datas, then creates a PivotTable report base on it.
 Dim sourceSheet As WebWorksheet =  GridWeb1.WebWorksheets("Sheet1")
 Dim sourceRange As Aspose.Cells.GridWeb.Data.WebCellArea =  New WebCellArea()/
 sourceRange.StartRow = 0
 sourceRange.StartColumn = 0
 sourceRange.EndRow = 10
 sourceRange.EndColumn = 5

 Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(sourceSheet,sourceRange)

 Dim table As PivotTable =  cache.CreatePivotTable()

 table.PivotFields(0).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(1).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(2).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(3).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField
 table.PivotFields(4).Orientation = PivotFieldOrientation.ColumnField
 table.PivotFields(5).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField

 table.PivotFields(3).Function = PivotFieldFunction.Count
 table.PivotFields(5).Function = PivotFieldFunction.Sum

 table.DataBind()

 'Creates a PivotTable report from DataView or DataTable.

 Dim dataView As DataView ' Or Dim dataTable As DataTable
     .
     .
 Sets dataView(dataTable) Value
     .
     .
     .

 Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(dataView)
 'Or Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(dataTable)
 Dim table As PivotTable =  cache.CreatePivotTable()
 table = GridWeb1.WebWorksheets.PivotTables("PivotTable1")
 table.PivotFields(0).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(1).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(2).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField
 table.DataBind()

```

### См. также

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


