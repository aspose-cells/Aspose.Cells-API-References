---
title: "Класс AutoFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.AutoFilter. Представляет автоматическую фильтрацию для указанного листа"
type: docs
url: /ru/net/aspose.cells/autofilter/
---
## AutoFilter class

Представляет автофильтрацию для указанного листа.

```csharp
public class AutoFilter
```

## Свойства

| Имя | Описание |
| --- | --- |
| [FilterColumns](../../aspose.cells/autofilter/filtercolumns/) { get; } | Получает коллекцию столбцов фильтра. |
| [Range](../../aspose.cells/autofilter/range/) { get; set; } | Представляет диапазон, к которому применяется указанный AutoFilter. |
| [ShowFilterButton](../../aspose.cells/autofilter/showfilterbutton/) { get; set; } | Указывает, видна ли кнопка AutoFilter для этого столбца. |
| [Sorter](../../aspose.cells/autofilter/sorter/) { get; } | Получает сортировщик данных. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddDateFilter](../../aspose.cells/autofilter/adddatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Добавляет фильтр по дате. |
| [AddFillColorFilter](../../aspose.cells/autofilter/addfillcolorfilter/)(int, BackgroundType, CellsColor, CellsColor) | Добавляет фильтр по цвету заливки. |
| [AddFilter](../../aspose.cells/autofilter/addfilter/)(int, string) | Добавляет фильтр для столбца фильтра. |
| [AddFontColorFilter](../../aspose.cells/autofilter/addfontcolorfilter/)(int, CellsColor) | Добавляет фильтр по цвету шрифта. |
| [AddIconFilter](../../aspose.cells/autofilter/addiconfilter/)(int, IconSetType, int) | Добавляет фильтр по значку. |
| [Custom](../../aspose.cells/autofilter/custom/#custom)(int, FilterOperatorType, object) | Фильтрует список с пользовательским критерием. |
| [Custom](../../aspose.cells/autofilter/custom/#custom_1)(int, FilterOperatorType, object, bool, FilterOperatorType, object) | Фильтрует список с пользовательскими критериями. |
| [DynamicFilter](../../aspose.cells/autofilter/dynamicfilter/)(int, DynamicFilterType) | Добавляет динамический фильтр. |
| [Filter](../../aspose.cells/autofilter/filter/)(int, string) | Фильтрует список с указанными критериями. |
| [FilterTop10](../../aspose.cells/autofilter/filtertop10/)(int, bool, bool, int) | Отфильтровать 10 лучших элементов в списке |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea)() | Получает [`CellArea`](../cellarea/), к которому применяется этот AutoFilter. |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea_1)(bool) | Получает [`CellArea`](../cellarea/), к которому применяется указанный AutoFilter. |
| [MatchBlanks](../../aspose.cells/autofilter/matchblanks/)(int) | Соответствует всем пустым ячейкам в списке. |
| [MatchNonBlanks](../../aspose.cells/autofilter/matchnonblanks/)(int) | Соответствует всем непустым ячейкам в списке. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh)() | Обновить автофильтры, чтобы скрыть или показать строки. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh_1)(bool) | Получает индексы всех скрытых строк. |
| [RemoveDateFilter](../../aspose.cells/autofilter/removedatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Удаляет фильтр по дате. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter)(int) | Удалить конкретный фильтр. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter_1)(int, string) | Удаляет фильтр для столбца фильтра. |
| [SetRange](../../aspose.cells/autofilter/setrange/)(int, int, int) | Устанавливает диапазон, к которому применяется указанный AutoFilter. |
| [ShowAll](../../aspose.cells/autofilter/showall/)() | Отобразить все скрытые строки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterDemo
    {
        public static void AutoFilterExample()
        {
            // Создание файлового потока, содержащего файл Excel, который будет открыт
            // Создание объекта Workbook
            Workbook workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Доступ к первому листу в файле Excel
            Worksheet worksheet = workbook.Worksheets[0];
            // Создание AutoFilter, задавая диапазон ячеек строки заголовка
            worksheet.AutoFilter.Range = "A1:B8";
            // Фильтрация столбцов с указанными значениями
            worksheet.AutoFilter.Filter(0, "Bananas");
            worksheet.AutoFilter.Refresh();

            // Сохранение изменённого файла Excel.
            workbook.Save("AutoFilterExample.xlsx");
            workbook.Save("AutoFilterExample.pdf");

            // Создание объекта Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Доступ к первому листу в файле Excel
            worksheet = workbook.Worksheets[0];

            // Дополнительный код для демонстрации других функций AutoFilter
            // Установка диапазона для AutoFilter
            worksheet.AutoFilter.Range = "A1:B8";
            // Добавление фильтра
            worksheet.AutoFilter.AddFilter(0, "Apples");
            // Добавление фильтра по дате
            worksheet.AutoFilter.AddDateFilter(1, DateTimeGroupingType.Year, 2022, 0, 0, 0, 0, 0);

            worksheet.AutoFilter.Refresh();
            // Сохранение изменённого файла Excel.
            workbook.Save("AutoFilterExample2.xlsx");
            workbook.Save("AutoFilterExample2.pdf");

            // Создание объекта Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Доступ к первому листу в файле Excel
            worksheet = workbook.Worksheets[0];
                        
            // Добавление фильтра по цвету шрифта
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Red;

            worksheet.AutoFilter.AddFontColorFilter(0, color);

            worksheet.AutoFilter.Refresh();
            // Сохранение изменённого файла Excel.
            workbook.Save("AutoFilterExample3.xlsx");
            workbook.Save("AutoFilterExample3.pdf");

            // Создание объекта Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Доступ к первому листу в файле Excel
            worksheet = workbook.Worksheets[0];

            // Добавление фильтра по цвету заливки
            CellsColor foregroundColor = workbook.CreateCellsColor();
            foregroundColor.Color = System.Drawing.Color.Red;
            CellsColor backgroundColor = workbook.CreateCellsColor();
            backgroundColor.Color = System.Drawing.Color.White;

            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, foregroundColor, backgroundColor);

            worksheet.AutoFilter.Refresh();
            // Сохранение изменённого файла Excel.
            workbook.Save("AutoFilterExample4.xlsx");
            workbook.Save("AutoFilterExample4.pdf");

            // Создание объекта Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Доступ к первому листу в файле Excel
            worksheet = workbook.Worksheets[0];

            // Сопоставление пустых ячеек
            worksheet.AutoFilter.MatchBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Сохранение изменённого файла Excel.
            workbook.Save("AutoFilterExample5.xlsx");
            workbook.Save("AutoFilterExample5.pdf");

            // Создание объекта Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Доступ к первому листу в файле Excel
            worksheet = workbook.Worksheets[0];

            // Сопоставление непустых ячеек
            worksheet.AutoFilter.MatchNonBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Сохранение изменённого файла Excel.
            workbook.Save("AutoFilterExample6.xlsx");
            workbook.Save("AutoFilterExample6.pdf");

            // Создание объекта Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Доступ к первому листу в файле Excel
            worksheet = workbook.Worksheets[0];

            // Пользовательский фильтр
            worksheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "Test");

            worksheet.AutoFilter.Refresh();
            // Сохранение изменённого файла Excel.
            workbook.Save("AutoFilterExample7.xlsx");
            workbook.Save("AutoFilterExample7.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


