---
title: "Cells.StandardWidthInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Получает или задает ширину столбца по умолчанию в листе в единицах дюймов"
type: docs
url: /ru/net/aspose.cells/cells/standardwidthinch/
---
## Cells.StandardWidthInch property

Получает или задает ширину столбца по умолчанию в листе, в единицах дюймов.

```csharp
public double StandardWidthInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить стандартную ширину столбца в дюймах
            worksheet.Cells.StandardWidthInch = 1.5;

            // Установить конкретную ширину столбца в дюймах для демонстрации
            worksheet.Cells.SetColumnWidthInch(1, 2.0);

            // Сохраните книгу
            workbook.Save("StandardWidthInchDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


