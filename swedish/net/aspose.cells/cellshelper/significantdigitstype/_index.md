---
title: "CellsHelper.SignificantDigitsType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-egenskap. Hämtar och anger standardtypen för signifikanta siffror vid utskrift av numeriska värden. Standardvärdet är G17"
type: docs
url: /sv/net/aspose.cells/cellshelper/significantdigitstype/
---
## CellsHelper.SignificantDigitsType property

Hämtar och anger standardtypen av signifikanta siffror för utskrift av numeriska värden. Standardvärdet är G17.

```csharp
public static SignificantDigitsType SignificantDigitsType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Visa det aktuella värdet för SignificantDigitsType
                Console.WriteLine("Current SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Ange ett nytt värde för SignificantDigitsType
                CellsHelper.SignificantDigitsType = SignificantDigitsType.G17;
                Console.WriteLine("Updated SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Skapa en arbetsbok för att demonstrera effekten
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till ett numeriskt värde som kommer att påverkas av signifikanta siffror
                worksheet.Cells["A1"].PutValue(1.2345678912345678);
                worksheet.Cells["A2"].PutValue(1.2345678912345678);
                worksheet.Cells["A3"].Formula = "=A1+A2";

                // Beräkna formler med den aktuella typen av signifikanta siffror
                workbook.CalculateFormula();

                // Visa resultatet
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].Value);

                // Byt till en annan typ av signifikanta siffror
                CellsHelper.SignificantDigitsType = SignificantDigitsType.Rounding17;
                Console.WriteLine("Changed SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Beräkna om med den nya typen av signifikanta siffror
                workbook.CalculateFormula();
                Console.WriteLine("Recalculated result: " + worksheet.Cells["A3"].Value);

                // Spara arbetsboken
                workbook.Save("SignificantDigitsTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


