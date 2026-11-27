---
title: "FormatCondition.SetFormula2"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition-metod. Anger värdet eller uttrycket som är kopplat till detta formatvillkor"
type: docs
url: /sv/net/aspose.cells/formatcondition/setformula2/
---
## FormatCondition.SetFormula2 method

Anger värdet eller uttrycket som är kopplat till detta formatvillkor.

```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
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

    public class FormatConditionMethodSetFormula2WithStringBooleanBooleanDemo
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

            // Lägg till ett formatvillkor
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Hämta det första formatvillkoret
            FormatCondition fc = fcs[0];

            try
            {
                // Anropa SetFormula2 med parametrarna (String, Boolean, Boolean)
                fc.SetFormula2("25", false, false);

                // Visa resultatet
                Console.WriteLine("SetFormula2 executed successfully. New Formula2: " + fc.Formula2);
                Console.WriteLine("Cells A1:A4 will be formatted if their values are between 10 and 25");

                // Applicera någon stil för att göra effekten synlig
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightGreen;
                fc.Style = style;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula2 method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("FormatConditionSetFormula2Demo.xlsx");
        }
    }
}
```

### Se även

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


