---
title: "Класс InsertOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.InsertOptions. Представляет параметры вставки"
type: docs
url: /ru/net/aspose.cells/insertoptions/
---
## InsertOptions class

Представляет параметры вставки.

```csharp
public class InsertOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [InsertOptions](insertoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CopyFormatType](../../aspose.cells/insertoptions/copyformattype/) { get; set; } |  |
| [FormulaChangeMonitor](../../aspose.cells/insertoptions/formulachangemonitor/) { get; set; } | Получает/задаёт монитор для отслеживания изменений, вызванных вставкой. |
| [UpdateReference](../../aspose.cells/insertoptions/updatereference/) { get; set; } | Указывает, будут ли обновляться ссылки в других листах. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InsertOptionsDemo
    {
        public static void InsertOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр InsertOptions
            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // Определите область ячеек, в которую будут вставляться строки
            CellArea cellArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };

            // Вставьте строки с указанными параметрами
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            // Сохраните книгу
            workbook.Save("InsertOptionsExample.xlsx");
            workbook.Save("InsertOptionsExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


