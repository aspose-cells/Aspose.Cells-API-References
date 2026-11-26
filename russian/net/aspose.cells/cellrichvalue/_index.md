---
title: "Класс CellRichValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CellRichValue. Представляет расширенное значение ячейки"
type: docs
url: /ru/net/aspose.cells/cellrichvalue/
---
## CellRichValue class

Представляет расширенное значение ячейки.

```csharp
public abstract class CellRichValue
```

## Свойства

| Имя | Описание |
| --- | --- |
| virtual [AltText](../../aspose.cells/cellrichvalue/alttext/) { get; set; } | Получает альтернативный текст, связанный с изображением. |
| virtual [ErrorValue](../../aspose.cells/cellrichvalue/errorvalue/) { get; } | Получает тип значения ошибки ячейки. |
| virtual [Image](../../aspose.cells/cellrichvalue/image/) { get; } | Получает данные изображения ячейки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassCellRichValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить расширенное значение в ячейку A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Rich Value");
            
            // Получить расширенное значение из ячейки A1
            CellRichValue richValue = cell.GetRichValue();
            
            // Отобразить свойства расширенного значения
            Console.WriteLine("Rich Value: " + richValue.ToString());
            
            // Сохраните книгу
            workbook.Save("RichValueDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


