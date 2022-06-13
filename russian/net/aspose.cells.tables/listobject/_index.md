---
title: ListObject
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет объект списка на рабочем листе. Объект ListObject является членом коллекции ListObjects. Коллекция ListObjects содержит все объекты списка на рабочем листе.
type: docs
weight: 5820
url: /ru/net/aspose.cells.tables/listobject/
---
## ListObject class

Представляет объект списка на рабочем листе. Объект ListObject является членом коллекции ListObjects. Коллекция ListObjects содержит все объекты списка на рабочем листе.

```csharp
public class ListObject
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription) { get; set; } | Получает и задает альтернативное описание. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext) { get; set; } | Получает и задает альтернативный текст. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter) { get; } | Получает автоматический фильтр. |
| [Comment](../../aspose.cells.tables/listobject/comment) { get; set; } | Получает и устанавливает комментарий к таблице. |
| [DataRange](../../aspose.cells.tables/listobject/datarange) { get; } | Получает диапазон данных ListObject. |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype) { get; } | Получает тип источника данных таблицы. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname) { get; set; } | Получает и задает отображаемое имя. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn) { get; } | Получает конечный столбец диапазона. |
| [EndRow](../../aspose.cells.tables/listobject/endrow) { get; } | Получает конечную строку диапазона. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns) { get; } | Получает ListColumns объекта ListObject. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable) { get; } | Получает связанную таблицу запросов. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow) { get; set; } | Получает и устанавливает, показывает ли этот ListObject строку заголовка. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes) { get; set; } | Указывает, применяется ли форматирование чередования столбцов. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn) { get; set; } | Указывает, следует ли применять стиль к первому столбцу таблицы. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn) { get; set; } | Указывает, следует ли применять стиль к последнему столбцу таблицы. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes) { get; set; } | Указывает, применяется ли форматирование чередования строк. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals) { get; set; } | Получает и устанавливает, показывает ли этот ListObject общую строку. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn) { get; } | Получает начальный столбец диапазона. |
| [StartRow](../../aspose.cells.tables/listobject/startrow) { get; } | Получает начальную строку диапазона. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename) { get; set; } | Получает и задает имя стиля таблицы. |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype) { get; set; } | Получает и встроенный стиль таблицы. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap) { get; } | Получает[`XmlMap`](./xmlmap)используемый для этого списка. |

## Методы

| Имя | Описание |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange)() | Применить стиль таблицы к диапазону. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange)() | Преобразование таблицы в диапазон. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange_1)(TableToRangeOptions) | Преобразование таблицы в диапазон. |
| [Filter](../../aspose.cells.tables/listobject/filter)() | Отфильтровать таблицу. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue)(int, int, object) | Поместите значение в ячейку. |
| [Resize](../../aspose.cells.tables/listobject/resize)(int, int, int, int, bool) | Изменение размера диапазона объекта списка. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname)() | Обновляет имена всех столбцов списка из рабочего листа. |

### Примеры

```csharp

[C#]


Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
for (int i = 0; i  <5; i++)
{
cells[0,i].PutValue(CellsHelper.ColumnIndexToName(i));
 }
for (int row = 1; row  <10; row++)
{
 for (int column = 0; column  <5; column++)
{
cells[row, column].PutValue(row * column);
 }
 }
ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[0];
table.ShowTotals = true;
table.ListColumns[4].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
workbook.Save(@"Book1.xlsx");


[Visual Basic]

Dim workbook As Workbook = New Workbook()
Dim cells As Cells = workbook.Worksheets(0).Cells
For i As Int32 = 0 To 4
 cells(0, i).PutValue(CellsHelper.ColumnIndexToName(i))
Next
For row As Int32 = 1 To 9
 For column As Int32 = 0 To 4
  cells(row, column).PutValue(row * column)
Next
Next
Dim tables As ListObjectCollection = workbook.Worksheets(0).ListObjects
Dim index As Int32 = tables.Add(0, 0, 9, 4, True)
Dim table As ListObject = tables(0)
table.ShowTotals = True
table.ListColumns(4).TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum
workbook.Save("Book1.xlsx")
```

### Смотрите также

* пространство имен [Aspose.Cells.Tables](../../aspose.cells.tables)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
