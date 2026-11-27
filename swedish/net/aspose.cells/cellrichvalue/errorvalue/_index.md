---
title: "CellRichValue.ErrorValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellRichValue-egenskap. Hämtar felvärdestypen för cellen"
type: docs
url: /sv/net/aspose.cells/cellrichvalue/errorvalue/
---
## CellRichValue.ErrorValue property

Hämtar felvärdestypen för cellen.

```csharp
public virtual ErrorCellValueType ErrorValue { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellRichValuePropertyErrorValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett spill‑fel i cell A1
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3})";
            
            try
            {
                // Beräkna formler för att generera spill‑felet
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // Förväntat spill-fel
            }
            
            // Hämta rikvärde från cell A1
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // Kontrollera och visa feltypen
            Console.WriteLine("Error type: " + richValue.ErrorValue);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* enum [ErrorCellValueType](../../errorcellvaluetype/)
* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


