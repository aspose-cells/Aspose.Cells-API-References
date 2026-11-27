---
title: "CalculationOptions.CalculationMonitor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationOptions-egenskap. Övervakaren som låter användaren följa framstegen i formelberäkning"
type: docs
url: /sv/net/aspose.cells/calculationoptions/calculationmonitor/
---
## CalculationOptions.CalculationMonitor property

Övervakaren för användaren att följa framstegen i formelberäkning.

```csharp
public AbstractCalculationMonitor CalculationMonitor { get; set; }
```

### Exempel

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCalculationMonitorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in några exempelformler
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Skapa beräkningsalternativ med en anpassad övervakare
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new SampleCalculationMonitor();

            // Beräkna formler med övervakning
            workbook.CalculateFormula(options);

            // Skriv ut resultat
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("A2: " + worksheet.Cells["A2"].Value);
            Console.WriteLine("A3: " + worksheet.Cells["A3"].Value);
        }
    }

    public class SampleCalculationMonitor : AbstractCalculationMonitor
    {
        public override bool OnCircular(IEnumerator circularCellsData)
        {
            // Hantera cirkulära referenser om det behövs
            return base.OnCircular(circularCellsData);
        }

        public override void BeforeCalculate(int sheetIndex, int rowIndex, int columnIndex)
        {
            Console.WriteLine($"Before calculation: Sheet{sheetIndex}, Row{rowIndex}, Col{columnIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int columnIndex)
        {
            Console.WriteLine($"After calculation: Sheet{sheetIndex}, Row{rowIndex}, Col{columnIndex}");
        }
    }
}
```

### Se även

* class [AbstractCalculationMonitor](../../abstractcalculationmonitor/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


