---
title: "Класс PivotCaches"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.Data.PivotCaches. Представляет коллекцию кэш‑памяти из отчётов PivotTable в рабочей книге. Каждый кэш памяти представлен объектом PivotCache."
type: docs
url: /ru/net/aspose.cells.gridweb.data/pivotcaches/
---
## PivotCaches class

Представляет коллекцию кэш‑памяти из отчётов PivotTable в рабочей книге. Каждый кэш памяти представлен объектом [`PivotCache`](../pivotcache/).

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotCaches : ICollection
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotcaches/count/) { get; } | Возвращает количество элементов, содержащихся в экземпляре PivotCaches. |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotcaches/issynchronized/) { get; } | Возвращает значение, указывающее, синхронизирован ли доступ к PivotCaches (потокобезопасный). |
| [Item](../../aspose.cells.gridweb.data/pivotcaches/item/) { get; } | Получает объект PivotCache по индексу. (2 индексатора) |
| [Parent](../../aspose.cells.gridweb.data/pivotcaches/parent/) { get; } | Получает родительский объект для указанного объекта. Только для чтения. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotcaches/syncroot/) { get; } | Возвращает объект, который может использоваться для синхронизации доступа к PivotCaches. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_2)(DataTable) | Добавляет PivotCache из DataTable. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_4)(DataView) | Добавляет PivotCache из DataView. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_3)(DataTable, string) | Добавляет PivotCahe из DataTable, используя указанное имя. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_5)(DataView, string) | Добавляет PivotCahe из DataView, используя указанное имя. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add)(WebWorksheet, WebCellArea) | Добавляет PivotCache из листа |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_1)(WebWorksheet, WebCellArea, string) | Добавляет PivotCache из листа, используя указанное имя. |
| [Clear](../../aspose.cells.gridweb.data/pivotcaches/clear/)() | Удаляет все объекты PivotCache и все объекты PivotTable в элементе управления. |
| [CopyTo](../../aspose.cells.gridweb.data/pivotcaches/copyto/)(Array, int) | Копирует весь PivotCache в совместимый одномерный массив Array, начиная с указанного индекса целевого массива. |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotcaches/getenumerator/)() | Возвращает IEnumerator для PivotCaches. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotcaches/indexof/)(PivotCache) | Возвращает индекс указанного PivotCache в коллекции. |
| [Remove](../../aspose.cells.gridweb.data/pivotcaches/remove/)(PivotCache) | Удаляет указанный объект PivotCache из PivotCaches и связанный PivotTable, используя pivotCache в качестве источника данных. |
| [RemoveAt](../../aspose.cells.gridweb.data/pivotcaches/removeat/)(int) | Удаляет указанный объект PivotCache из PivotCaches и связанный PivotTable, используя pivotCache в качестве источника данных. |

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


