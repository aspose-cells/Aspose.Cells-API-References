---
title: "Класс FilterColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.FilterColumn. Представляет фильтр для отдельного столбца или столбца в таблице"
type: docs
url: /ru/net/aspose.cells/filtercolumn/
---
## FilterColumn class

Представляет фильтр для отдельного столбца или столбца в таблице.

```csharp
public class FilterColumn
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ColorFilter](../../aspose.cells/filtercolumn/colorfilter/) { get; } | Получает [`ColorFilter`](../colorfilter/) для фильтрации данных по цвету. |
| [CustomFilters](../../aspose.cells/filtercolumn/customfilters/) { get; set; } | Получает [`CustomFilterCollection`](../customfiltercollection/) для фильтрации данных по пользовательским критериям. |
| [DynamicFilter](../../aspose.cells/filtercolumn/dynamicfilter/) { get; } | Получает [`DynamicFilter`](./dynamicfilter/) для фильтрации с динамическими критериями. |
| [FieldIndex](../../aspose.cells/filtercolumn/fieldindex/) { get; set; } | Получает и задает смещение столбца в диапазоне. |
| [Filter](../../aspose.cells/filtercolumn/filter/) { get; set; } | (**Obsolete.**) Получает и задает условие фильтрации данных. |
| [FilterType](../../aspose.cells/filtercolumn/filtertype/) { get; set; } | Получает и задает тип фильтрации данных. |
| [FilterValues](../../aspose.cells/filtercolumn/filtervalues/) { get; } | Получает [`FilterValueCollection`](../filtervaluecollection/) для фильтрации данных по меткам или дате и времени. |
| [IconFilter](../../aspose.cells/filtercolumn/iconfilter/) { get; } | Получает [`IconFilter`](./iconfilter/) для фильтрации данных по значку. |
| [IsDropdownVisible](../../aspose.cells/filtercolumn/isdropdownvisible/) { get; set; } | Указывает, видна ли кнопка AutoFilter для этого столбца. |
| [MultipleFilters](../../aspose.cells/filtercolumn/multiplefilters/) { get; set; } | (**Obsolete.**) Получает [`MultipleFilterCollection`](../multiplefiltercollection/) для фильтрации данных по меткам или дате и времени. |
| [Top10Filter](../../aspose.cells/filtercolumn/top10filter/) { get; } | Получает [`Top10Filter`](./top10filter/) для фильтрации данных по рангу. |

## Методы

| Имя | Описание |
| --- | --- |
| [SelectAll](../../aspose.cells/filtercolumn/selectall/)() | Выбирает всё. |

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;

namespace AsposeCellsExamples
{
    public class FilterColumnDemo
    {
        public static void RunDemo()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Jane");
            sheet.Cells["A4"].PutValue("Doe");

            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(25);
            sheet.Cells["B4"].PutValue(35);

            // Применить автофильтр к диапазону
            sheet.AutoFilter.SetRange(0, 0, 3);

            // Добавить фильтр к первому столбцу (Name)
            sheet.AutoFilter.AddFilter(0, "John");

            // Добавить фильтр к второму столбцу (Age)
            sheet.AutoFilter.AddFilter(1, "30");

            // Обновить фильтр, чтобы применить его
            sheet.AutoFilter.Refresh();

            // Получить доступ к FilterColumnCollection
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // Получить доступ к первому FilterColumn
            FilterColumn filterColumn = filterColumns[0];

            // Отобразить свойства FilterColumn
            Console.WriteLine($"IsDropdownVisible: {filterColumn.IsDropdownVisible}");
            Console.WriteLine($"Filter: {filterColumn.Filter}");
            Console.WriteLine($"FilterType: {filterColumn.FilterType}");
            Console.WriteLine($"FieldIndex: {filterColumn.FieldIndex}");

            // Сохраните книгу
            workbook.Save("FilterColumnDemo.xlsx");
            workbook.Save("FilterColumnDemo.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


