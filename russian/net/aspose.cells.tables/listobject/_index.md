---
title: "Класс ListObject"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Tables.ListObject. Представляет таблицу в листе"
type: docs
url: /ru/net/aspose.cells.tables/listobject/
---
## ListObject class

Представляет таблицу в листе.

```csharp
public class ListObject
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription/) { get; set; } | Получает и задает альтернативное описание. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext/) { get; set; } | Получает и задает альтернативный текст. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter/) { get; } | Получает автофильтр этой таблицы. |
| [Comment](../../aspose.cells.tables/listobject/comment/) { get; set; } | Получает и задает комментарий таблицы. |
| [DataRange](../../aspose.cells.tables/listobject/datarange/) { get; } | Получает диапазон данных таблицы. |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype/) { get; } | Получает тип источника данных таблицы. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname/) { get; set; } | Получает и задает отображаемое имя таблицы. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn/) { get; } | Получает конечный столбец диапазона. |
| [EndRow](../../aspose.cells.tables/listobject/endrow/) { get; } | Получает конечную строку диапазона. |
| [HasAutoFilter](../../aspose.cells.tables/listobject/hasautofilter/) { get; set; } | Указывает, применён ли автофильтр к этой таблице. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns/) { get; } | Получает список [`ListColumn`](../listcolumn/) этой таблицы. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable/) { get; } | Получает связанную QueryTable. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow/) { get; set; } | Получает и задает, отображает ли эта таблица строку заголовка. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes/) { get; set; } | Указывает, применяется ли форматирование полос столбцов к. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn/) { get; set; } | Указывает, применяется ли стиль к первому столбцу в таблице. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn/) { get; set; } | Указывает, применяется ли стиль к последнему столбцу в таблице. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes/) { get; set; } | Указывает, применяется ли форматирование полос строк к. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals/) { get; set; } | Получает и задает, отображает ли эта TAble строку итогов. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn/) { get; } | Получает начальный столбец диапазона. |
| [StartRow](../../aspose.cells.tables/listobject/startrow/) { get; } | Получает начальную строку диапазона. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename/) { get; set; } | Получает и задает имя стиля таблицы |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype/) { get; set; } | Получает встроенный стиль таблицы. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap/) { get; } | Получает [`XmlMap`](./xmlmap/) используемый для этого списка. |

## Методы

| Имя | Описание |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange/)() | Применить стиль таблицы к диапазону. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange)() | Преобразовать таблицу в диапазон. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange_1)(TableToRangeOptions) | Преобразовать таблицу в диапазон. |
| [Filter](../../aspose.cells.tables/listobject/filter/)() | (**Устарело.**) Фильтровать таблицу. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula)(int, int, string) | Поместить формулу в ячейку таблицы. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula_1)(int, int, string, bool) | Поместить формулу в ячейку таблицы. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue)(int, int, object) | Поместить значение в ячейку. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue_1)(int, int, object, bool) | Поместить значение в ячейку. |
| [RemoveAutoFilter](../../aspose.cells.tables/listobject/removeautofilter/)() | Удаляет автофильтр, примененный к этой таблице. |
| [Resize](../../aspose.cells.tables/listobject/resize/)(int, int, int, int, bool) | Изменить размер диапазона объекта списка. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname/)() | Обновляет имена всех столбцов списка в ячейках таблицы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectDemo
    {
        public static void ListObjectExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Заполните лист некоторыми данными
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Добавить объект ListObject (таблицу) в лист
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Установить некоторые свойства ListObject
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;
            table.DisplayName = "SampleTable";
            table.Comment = "This is a sample table.";
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.ShowTableStyleRowStripes = true;
            table.ShowTableStyleColumnStripes = true;
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Сохраните книгу
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


