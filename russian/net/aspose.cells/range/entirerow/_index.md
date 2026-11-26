---
title: "Range.EntireRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Возвращает объект Range, представляющий всю строку или строки, содержащие указанный диапазон"
type: docs
url: /ru/net/aspose.cells/range/entirerow/
---
## Range.EntireRow property

Получает объект Range, представляющий всю строку (или строки), содержащую указанный диапазон.

```csharp
public Range EntireRow { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Заполните некоторыми образцами данных первую строку
            for (int col = 0; col < 5; col++)
            {
                sheet.Cells[0, col].PutValue($"Header {col + 1}");
            }

            // Получите всю первую строку, используя свойство EntireRow
            Aspose.Cells.Range entireRow = sheet.Cells.CreateRange("A1").EntireRow;

            // Скопируйте первую строку в третью строку
            Aspose.Cells.Range destination = sheet.Cells.CreateRange("A3").EntireRow;
            destination.Copy(entireRow);

            // Сохраните книгу
            workbook.Save("EntireRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


