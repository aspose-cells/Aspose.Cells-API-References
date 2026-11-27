---
title: "CalculationData.Workbook"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationData-egenskap. Hämtar Workbook-objektet där funktionen finns"
type: docs
url: /sv/net/aspose.cells/calculationdata/workbook/
---
## CalculationData.Workbook property

Hämtar Workbook-objektet där funktionen är.

```csharp
public Workbook Workbook { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata och formel
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].Formula = "=CUSTOMFUNC()";

            // Skapa beräkningsalternativ och registrera anpassad beräkningsmotor
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalcEngine();

            // Starta beräkning med alternativ för att demonstrera användning av Workbook-egenskapen
            workbook.CalculateFormula(options);

            // Visa resultatet från beräkningen
            Console.WriteLine("Calculated value in B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("Modified value in C1: " + worksheet.Cells["C1"].Value);

            // Spara resultatet
            workbook.Save("PropertyWorkbookDemo.xlsx");
        }

        private class CustomCalcEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "CUSTOMFUNC")
                {
                    // Åtkomst till Workbook-egenskapen från CalculationData
                    Workbook currentWorkbook = data.Workbook;
                    Worksheet currentSheet = currentWorkbook.Worksheets[0];

                    // Demonstrera användning av workbook för att manipulera data
                    double inputValue = (double)currentSheet.Cells["A1"].Value;
                    currentSheet.Cells["C1"].PutValue(inputValue * 2);

                    // Ange beräknat resultat
                    data.CalculatedValue = inputValue * 3;
                }
            }
        }
    }
}
```

### Se även

* class [Workbook](../../workbook/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


