---
title: "Cell.IsErrorValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑egenskap. Kontrollerar om värdet i den här cellen är ett fel"
type: docs
url: /sv/net/aspose.cells/cell/iserrorvalue/
---
## Cell.IsErrorValue property

Kontrollerar om värdet i den här cellen är ett fel.

```csharp
public bool IsErrorValue { get; }
```

### Anmärkningar

Gäller också för formelceller för att kontrollera om det beräknade resultatet är ett fel.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsErrorValueDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in en formel som kommer att resultera i ett fel
            Cell cell = cells["A1"];
            cell.Formula = "=1/0"; // Division by zero error
            
            // Beräkna formler
            workbook.CalculateFormula();

            // Demonstrera IsErrorValue‑egenskapen
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("IsErrorValue: " + cell.IsErrorValue);
            Console.WriteLine("Error type: " + cell.Value);

            // Ange ett giltigt värde
            Cell cell2 = cells["A2"];
            cell2.PutValue("Valid value");
            
            Console.WriteLine("\nCell A2 value: " + cell2.StringValue);
            Console.WriteLine("IsErrorValue: " + cell2.IsErrorValue);

            // Ställ in ett SPILL‑fel (Excel 365+ dynamisk matrisformelfel)
            Cell cell3 = cells["A3"];
            cell3.SetDynamicArrayFormula("=A1:A10", new FormulaParseOptions(), true);
            
            Console.WriteLine("\nCell A3 value: " + cell3.StringValue);
            Console.WriteLine("IsErrorValue: " + cell3.IsErrorValue);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


