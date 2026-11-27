---
title: "Klass CalculationOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CalculationOptions‑klass. Representerar alternativ för beräkning"
type: docs
url: /sv/net/aspose.cells/calculationoptions/
---
## CalculationOptions class

Representerar alternativ för beräkning.

```csharp
public class CalculationOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [CalculationOptions](calculationoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CalcStackSize](../../aspose.cells/calculationoptions/calcstacksize/) { get; set; } | Stackstorleken för rekursiv beräkning av celler. Standardvärdet är 200. |
| [CalculationMonitor](../../aspose.cells/calculationoptions/calculationmonitor/) { get; set; } | Övervakaren för användaren att följa framstegen i formelberäkning. |
| [CharacterEncoding](../../aspose.cells/calculationoptions/characterencoding/) { get; set; } | Anger den kodning som används för kodning/avkodning av tecken vid beräkning av formler. För funktioner såsom CHAR, CODE beror det beräknade resultatet på regioninställningarna och standardteckenuppsättningen i miljön. Med den här egenskapen kan användaren ange rätt kodning som används för dessa funktioner för att få det förväntade resultatet. |
| [CustomEngine](../../aspose.cells/calculationoptions/customengine/) { get; set; } | Den anpassade formelberäkningsmotorn för att utöka standardberäkningsmotorn i Aspose.Cells. |
| [IgnoreError](../../aspose.cells/calculationoptions/ignoreerror/) { get; set; } | Anger om fel som uppstår vid beräkning av formler ska ignoreras. Felet kan vara en funktion som inte stöds, externa länkar osv. Standardvärdet är true. |
| [LinkedDataSources](../../aspose.cells/calculationoptions/linkeddatasources/) { get; set; } | Anger datakällorna för externa länkar som används i formler. |
| [PrecisionStrategy](../../aspose.cells/calculationoptions/precisionstrategy/) { get; set; } | Anger strategin för bearbetning av beräkningsprecision. |
| [Recursive](../../aspose.cells/calculationoptions/recursive/) { get; set; } | Anger om beroende celler ska beräknas rekursivt när en cell beräknas och den beror på andra celler. Standardvärdet är true. |
| [RefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/refreshdynamicarrayformula/) { get; set; } | Anger om dynamiska matrisformler ska uppdateras innan formler beräknas. |
| [UserSpecifiedRefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/) { get; } | Anger om användaren uttryckligen har specificerat beteendet för att uppdatera dynamiska matrisformler innan angivna formler beräknas. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class CalculationOptionsDemo
    {
        public static void CalculationOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue(10.555);
            worksheet.Cells["A2"].PutValue(20.6666);
            worksheet.Cells["A3"].PutValue(30.7777);
            worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";

            // Skapa en instans av CalculationOptions
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                CalcStackSize = 200,
                PrecisionStrategy = CalculationPrecisionStrategy.Round,
                CharacterEncoding = Encoding.UTF8
            };

            // Valfritt kan du ange en anpassad beräkningsmotor eller övervakare
            // calcOptions.CustomEngine = new MyCustomEngine();
            // calcOptions.CalculationMonitor = new MyCalculationMonitor();

            // Beräkna formler i arbetsboken med de angivna alternativen
            workbook.CalculateFormula(calcOptions);

            // Spara arbetsboken
            workbook.Save("CalculationOptionsExample.xlsx");
            workbook.Save("CalculationOptionsExample.pdf");

        }
    }

    // Exempel på anpassad beräkningsmotor (om behövs)
    public class MyCustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Anpassad beräkningslogik
            string funcName = data.FunctionName.ToUpper();
            if (funcName == "MYFUNC")
            {
                // Exempel på anpassad funktionslogik
                int count = data.ParamCount;
                object result = null;
                for (int i = 0; i < count; i++)
                {
                    object paramValue = data.GetParamValue(i);
                    if (paramValue is ReferredArea)
                    {
                        ReferredArea ra = (ReferredArea)paramValue;
                        paramValue = ra.GetValue(0, 0);
                    }
                    // Bearbeta parametern här
                    // result = ...;
                }
                data.CalculatedValue = result;
            }
        }
    }

    // Exempel på anpassad beräkningsövervakare (om behövs)
    public class MyCalculationMonitor : AbstractCalculationMonitor
    {
        public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // Logik före beräkning
            Console.WriteLine($"Before calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // Logik efter beräkning
            Console.WriteLine($"After calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override bool OnCircular(System.Collections.IEnumerator circularCellsData)
        {
            // Hantera cirkulära referenser
            Console.WriteLine("Circular reference detected.");
            return true; // Continue calculation
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


