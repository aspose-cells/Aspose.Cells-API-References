---
title: "Перечисление PasteOperationType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.PasteOperationType. Представляет тип операции при вставке диапазона"
type: docs
url: /ru/net/aspose.cells/pasteoperationtype/
---
## PasteOperationType enumeration

Представляет тип операции при вставке диапазона.

```csharp
public enum PasteOperationType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Нет операции. |
| Add | `1` | Добавить |
| Subtract | `2` | Вычесть |
| Multiply | `3` | Умножить |
| Divide | `4` | Разделить |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPasteOperationTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["B1"].PutValue(20);
            sheet.Cells["C1"].PutValue(30);
            
            // Создать параметры вставки с PasteOperationType.None
            var pasteOptions = new PasteOptions()
            {
                PasteType = PasteType.Values,
                OperationType = PasteOperationType.None,
                SkipBlanks = false,
                Transpose = false
            };

            // Создать диапазон и скопировать с параметрами вставки
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1", "C1");
            Aspose.Cells.Range destRange = sheet.Cells.CreateRange("A2", "C2");
            sourceRange.Copy(destRange, pasteOptions);

            // Сохраните книгу
            workbook.Save("PasteOperationTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


