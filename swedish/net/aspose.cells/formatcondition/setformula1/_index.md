---
title: "FormatCondition.SetFormula1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition-metod. Anger värdet eller uttrycket som är kopplat till detta formatvillkor"
type: docs
url: /sv/net/aspose.cells/formatcondition/setformula1/
---
## FormatCondition.SetFormula1 method

Anger värdet eller uttrycket som är kopplat till detta formatvillkor.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | Värdet eller uttrycket som är kopplat till detta formatvillkor. Om inmatningsvärdet börjar med '=', tas det som en formel. Annars tas det som ett vanligt värde (text, nummer, bool). För textvärden som börjar med '=', kan användaren ange det som formel i formatet: "=\"=...\"". |
| isR1C1 | Boolean | Om formeln är en R1C1-formel. |
| isLocal | Boolean | Om formeln är lokalt formaterad. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodSetFormula1WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Lägg till ett villkorsformateringsområde
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Hämta det första formatvillkoret
            FormatCondition fc = fcc[0];

            try
            {
                // Anropa SetFormula1 med parametrar (String, Boolean, Boolean)
                fc.SetFormula1("SUM(A1:A4)", false, false);

                // Visa resultatet
                Console.WriteLine("SetFormula1 executed successfully with formula: " + fc.Formula1);
                Console.WriteLine("Conditional formatting applied to range A1:A4 with formula: " + fc.Formula1);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1 method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("FormatConditionSetFormula1Demo.xlsx");
        }
    }
}
```

### Se även

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


