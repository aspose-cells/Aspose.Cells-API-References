---
title: "Cells.ConvertStringToNumericValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Konverterar all strängdata i kalkylbladet till numeriskt värde om möjligt"
type: docs
url: /sv/net/aspose.cells/cells/convertstringtonumericvalue/
---
## Cells.ConvertStringToNumericValue method

Konverterar all strängdata i kalkylbladet till numeriskt värde om möjligt.

```csharp
public void ConvertStringToNumericValue()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodConvertStringToNumericValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Placera strängvärden som kan konverteras till numeriska värden
            cells[0, 0].PutValue("1.23");
            cells[0, 1].PutValue("1.24");
            cells[0, 2].PutValue("1.23");
            cells[0, 3].PutValue("6/20/2021");
            cells[0, 4].PutValue("def"); // This will remain as string
            cells[0, 5].PutValue("6/20/2021");

            // Konvertera strängvärden till numeriska där det är möjligt
            cells.ConvertStringToNumericValue();

            // Visa de konverterade värdena
            Console.WriteLine("A1: " + cells[0, 0].DoubleValue);
            Console.WriteLine("B1: " + cells[0, 1].DoubleValue);
            Console.WriteLine("C1: " + cells[0, 2].DoubleValue);
            Console.WriteLine("D1: " + cells[0, 3].DoubleValue);
            Console.WriteLine("E1: " + cells[0, 4].StringValue); // Remains as string
            Console.WriteLine("F1: " + cells[0, 5].DoubleValue);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


