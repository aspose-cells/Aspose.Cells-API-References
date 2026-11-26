---
title: "Worksheet.ShowFormulas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Указывает, показывать формулы или их результаты"
type: docs
url: /ru/net/aspose.cells/worksheet/showformulas/
---
## Worksheet.ShowFormulas property

Указывает, показывать ли формулы или их результаты.

```csharp
public bool ShowFormulas { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyShowFormulasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить формулу в ячейку A1
            worksheet.Cells["A1"].Formula = "=1+2+3";
            
            // Изначально показывать вычисленное значение
            worksheet.ShowFormulas = false;
            Console.WriteLine("ShowFormulas OFF: " + worksheet.Cells["A1"].StringValue);

            // Переключить отображение текста формулы
            worksheet.ShowFormulas = true;
            Console.WriteLine("ShowFormulas ON: " + worksheet.Cells["A1"].StringValue);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


