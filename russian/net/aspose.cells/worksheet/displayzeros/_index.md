---
title: "Worksheet.DisplayZeros"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. True, если нулевые значения отображаются"
type: docs
url: /ru/net/aspose.cells/worksheet/displayzeros/
---
## Worksheet.DisplayZeros property

True, если отображаются нулевые значения.

```csharp
public bool DisplayZeros { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyDisplayZerosDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Продемонстрировать DisplayZeros = true (по умолчанию)
            sheet.DisplayZeros = true;
            Cell cell1 = sheet.Cells["A1"];
            cell1.PutValue(0);
            Console.WriteLine("DisplayZeros=true: " + cell1.StringValue);

            // Продемонстрировать DisplayZeros = false
            sheet.DisplayZeros = false;
            Cell cell2 = sheet.Cells["A2"];
            cell2.PutValue(0);
            Console.WriteLine("DisplayZeros=false: " + cell2.StringValue);

            // Показать пользовательское форматирование с DisplayZeros
            Style style = wb.CreateStyle();
            style.Custom = "0.00;\"Zero\";\"Negative\"";
            Cell cell3 = sheet.Cells["A3"];
            cell3.PutValue(0);
            cell3.SetStyle(style);
            Console.WriteLine("Custom format with DisplayZeros=true: " + cell3.StringValue);

            sheet.DisplayZeros = false;
            Cell cell4 = sheet.Cells["A4"];
            cell4.PutValue(0);
            cell4.SetStyle(style);
            Console.WriteLine("Custom format with DisplayZeros=false: " + cell4.StringValue);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


