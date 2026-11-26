---
title: "Класс PivotField"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridWeb.Data.PivotField class. Представляет поле в отчёте PivotTable. Объект PivotField является членом коллекции PivotFields.  ПРИМЕЧАНИЕ Этот класс теперь устарел. Вместо него используйте GridPivotField. Этот класс будет удалён через 6 месяцев после августа 2014 г. Aspose приносит извинения за любые неудобства, которые вы могли испытать"
type: docs
url: /ru/net/aspose.cells.gridweb.data/pivotfield/
---
## PivotField class

Представляет поле в отчёте PivotTable. Объект PivotField является членом коллекции [`PivotFields`](../pivotfields/).  ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него используйте GridPivotField. Этот класс будет удалён через 6 месяцев после августа 2014 г. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

```csharp
[Obsolete("This class is obsolete; use GridPivotField instead")]
public class PivotField
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Caption](../../aspose.cells.gridweb.data/pivotfield/caption/) { get; set; } | Текст метки для поля сводки отображается в отчёте. По умолчанию отображается имя. |
| [FieldItems](../../aspose.cells.gridweb.data/pivotfield/fielditems/) { get; } | Получает данные указанного поля. |
| [Function](../../aspose.cells.gridweb.data/pivotfield/function/) { get; set; } | Представляет функцию, используемую для суммирования поля PivotTable (только для полей данных). Функция по умолчанию — Count. |
| [Name](../../aspose.cells.gridweb.data/pivotfield/name/) { get; } | Получает имя. |
| [Orientation](../../aspose.cells.gridweb.data/pivotfield/orientation/) { get; set; } | Представляет расположение поля в указанном отчёте PivotTable. |
| [Position](../../aspose.cells.gridweb.data/pivotfield/position/) { get; set; } | Представляет позицию поля (первое, второе, третье и т.д.) среди всех полей в его ориентации (Rows, Columns, Pages). Вы должны вызвать метод get после вызова Pivottable.DataBind. |
| [SortOrder](../../aspose.cells.gridweb.data/pivotfield/sortorder/) { get; set; } | Представляет порядок, используемый для сортировки указанного поля PivotTable. |

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


