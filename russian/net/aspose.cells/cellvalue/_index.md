---
title: "Класс CellValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CellValue. Представляет значение ячейки и соответствующий тип."
type: docs
url: /ru/net/aspose.cells/cellvalue/
---
## CellValue class

Представляет значение ячейки и соответствующий тип.

```csharp
public class CellValue
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CellValue](cellvalue/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Type](../../aspose.cells/cellvalue/type/) { get; set; } | Получает или задает тип значения ячейки. |
| [Value](../../aspose.cells/cellvalue/value/) { get; set; } | Получает или задает значение ячейки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueDemo
    {
        public static void CellValueExample()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр CellValue
            CellValue cellValue = new CellValue();

            // Установите тип и значение ячейки
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            // Назначьте CellValue ячейке в рабочем листе
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(cellValue.Value);

            // Сохраните книгу
            workbook.Save("CellValueExample.xlsx");
            workbook.Save("CellValueExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


