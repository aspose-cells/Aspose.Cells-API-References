---
title: "Класс PivotFields"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.Data.PivotFields. Представляет коллекцию всех объектов PivotField в отчёте сводной таблицы"
type: docs
url: /ru/net/aspose.cells.gridweb.data/pivotfields/
---
## PivotFields class

Представляет коллекцию всех объектов [`PivotField`](../pivotfield/) в отчёте сводной таблицы.

```csharp
[Obsolete("This class is obsolete; use GridPivotFieldCollection instead")]
public class PivotFields : ICollection
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotfields/count/) { get; } | Получает количество элементов, содержащихся в экземпляре PivotFields |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotfields/issynchronized/) { get; } | Получает значение, указывающее, синхронизирован ли доступ к PivotFields (потокобезопасный). |
| [Item](../../aspose.cells.gridweb.data/pivotfields/item/) { get; } | Получает PivotField по индексу. (2 индексатора) |
| [Parent](../../aspose.cells.gridweb.data/pivotfields/parent/) { get; } | Получает родительский объект для указанного объекта. Только для чтения. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotfields/syncroot/) { get; } | Получает объект, который можно использовать для синхронизации доступа к PivotFields. |

## Методы

| Имя | Описание |
| --- | --- |
| [CopyTo](../../aspose.cells.gridweb.data/pivotfields/copyto/)(Array, int) | Копирует весь PivotField в совместимый одномерный массив, начиная с указанного индекса целевого массива |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotfields/getenumerator/)() | Возвращает IEnumerator для PivotFields. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotfields/indexof/)(PivotField) | Получает индекс указанного PivotField. |

### Примечания

ПРИМЕЧАНИЕ: Этот класс теперь устарел. пожалуйста, используйте вместо него GridPivotFieldCollection. Этот класс будет удалён через 6 месяцев после августа 2014 г. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp

 [C#]

 //Получает PivotFields из PivotTable[0]
 PivotField field1 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field1"];
 PivotField field2 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field2"];
 PivotField field3 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field3"];
 PivotField field4 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field4"];

 //Устанавливает расположение PivotFields
 field1.Orientation = PivotFieldOrientation.RowField;
 field2.Orientation = PivotFieldOrientation.RowField;
 field3.Orientation = PivotFieldOrientation.ColumnField;
 field4.Orientation = PivotFieldOrientation.DataField;

 //Устанавливает функцию поля данных
 field3.Function = PivotFieldFunction.Sum;

 //Изменяет порядок полей строки
 field2.Position = 1; //Or field1.Position = 2;

 [VB]

 'Gets PivotFields of PivotTable[0]
 Dim field1 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field1")
 Dim field2 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field2")
 Dim field3 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field3")
 Dim field4 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field4")

 'Sets Location of PivotFields
 field1.Orientation = PivotFieldOrientation.RowField
 field2.Orientation = PivotFieldOrientation.RowField
 field3.Orientation = PivotFieldOrientation.ColumnField
 field4.Orientation = PivotFieldOrientation.DataField

 'Sets function of data field
 field3.Function = PivotFieldFunction.Sum
 'Changes row fields order
 field2.Position = 1 'Or field1.Position = 2;

```

### См. также

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


