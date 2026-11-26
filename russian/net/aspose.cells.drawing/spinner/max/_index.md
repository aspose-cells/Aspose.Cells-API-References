---
title: "Spinner.Max"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Spinner. Получает или задает максимальное значение полосы прокрутки или диапазона спиннера"
type: docs
url: /ru/net/aspose.cells.drawing/spinner/max/
---
## Spinner.Max property

Получает или задает максимальное значение диапазона полосы прокрутки или спиннера.

```csharp
public int Max { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyMaxDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.Spinner spinner = sheet.Shapes.AddSpinner(1, 1, 0, 0, 100, 100);
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;

            Console.WriteLine($"Spinner Max Value: {spinner.Max}");
        }
    }
}
```

### См. также

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


