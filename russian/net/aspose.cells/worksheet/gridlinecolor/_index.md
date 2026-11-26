---
title: "Worksheet.GridlineColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает и задает цвет линий сетки"
type: docs
url: /ru/net/aspose.cells/worksheet/gridlinecolor/
---
## Worksheet.GridlineColor property

Получает и задаёт цвет линий сетки

```csharp
public Color GridlineColor { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить цвет линий сетки в красный
            worksheet.GridlineColor = Color.Red;
            
            // Сохраните книгу
            string outputPath = "GridlineColorDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Gridline color set to red and saved to: " + outputPath);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


