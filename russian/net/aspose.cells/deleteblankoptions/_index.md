---
title: "Класс DeleteBlankOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.DeleteBlankOptions. Представляет настройку удаления пустых ячеек/строк/столбцов"
type: docs
url: /ru/net/aspose.cells/deleteblankoptions/
---
## DeleteBlankOptions class

Представляет настройку удаления пустых ячеек/строк/столбцов.

```csharp
public class DeleteBlankOptions : DeleteOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [DeleteBlankOptions](deleteblankoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [DrawingsAsBlank](../../aspose.cells/deleteblankoptions/drawingsasblank/) { get; set; } | Указывает, будут ли графические объекты, такие как изображение, фигура, диаграмма..., считаться пустыми. Значение по умолчанию — true. |
| [EmptyFormulaValueAsBlank](../../aspose.cells/deleteblankoptions/emptyformulavalueasblank/) { get; set; } | Будет ли ячейка считаться пустой, если она содержит формулу, а вычисленный результат равен null или пустой строке. Значение по умолчанию — false. |
| [EmptyStringAsBlank](../../aspose.cells/deleteblankoptions/emptystringasblank/) { get; set; } | Указывает, будет ли ячейка считаться пустой, когда её значение — пустая строка. Значение по умолчанию — true. |
| [EndIndex](../../aspose.cells/deleteblankoptions/endindex/) { get; set; } | Задает конечный индекс строки/столбца (включительно) диапазона, который нужно проверить и удалить пустые строки/столбцы. Значение по умолчанию — -1, а -1 означает максимальный диапазон всех объектов (ячейки, рисунки, ...) которые необходимо проверить. |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Получает/устанавливает монитор для отслеживания изменений, вызванных удалением. (Наследуется от [`DeleteOptions`](../deleteoptions/).) |
| [MergedCellsShrinkType](../../aspose.cells/deleteblankoptions/mergedcellsshrinktype/) { get; set; } | Указывает, как обрабатывать объединённые ячейки при удалении пустых строк/столбцов. |
| [StartIndex](../../aspose.cells/deleteblankoptions/startindex/) { get; set; } | Задает начальный индекс строки/столбца диапазона, который нужно проверить и удалить пустую строку/столбец. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Указывает, следует ли обновлять ссылки в других листах. (Наследуется от [`DeleteOptions`](../deleteoptions/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteBlankOptionsDemo
    {
        public static void DeleteBlankOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните лист некоторыми данными
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // Создайте экземпляр DeleteBlankOptions
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true,
                EmptyFormulaValueAsBlank = false,
                UpdateReference = true
            };

            // Удалить пустые строки в соответствии с параметрами
            worksheet.Cells.DeleteBlankRows(options);

            // Сохраните книгу
            workbook.Save("DeleteBlankOptionsExample.xlsx");
            workbook.Save("DeleteBlankOptionsExample.pdf");
            return;
        }
    }
}
```

### См. также

* class [DeleteOptions](../deleteoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


