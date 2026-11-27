---
title: "ReferredArea.SheetNames"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReferredArea-egenskap. Namn på alla kalkylblad som detta objekt refererar till"
type: docs
url: /sv/net/aspose.cells/referredarea/sheetnames/
---
## ReferredArea.SheetNames property

Namn på alla kalkylblad som denna instans refererar till.

```csharp
public string[] SheetNames { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertySheetNamesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data för att skapa en formelreferens
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Beräkna formler för att få referenser
            workbook.CalculateFormula();

            // Hämta det refererade området från formeln i A3
            ReferredArea referredArea = worksheet.Cells["A3"].GetPrecedents()[0];

            // Visa SheetNames-egenskapen
            Console.WriteLine("SheetNames referenced by the formula:");
            if (referredArea.SheetNames != null)
            {
                foreach (string sheetName in referredArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // Lägg till ett annat kalkylblad och skapa en korsarkivreferens
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["B1"].PutValue("=Sheet1!A3");

            // Beräkna formler igen
            workbook.CalculateFormula();

            // Hämta det refererade området från korsarkivformeln
            ReferredArea crossSheetArea = sheet2.Cells["B1"].GetPrecedents()[0];

            // Visa SheetNames för korsarkivreferens
            Console.WriteLine("\nSheetNames referenced by cross-sheet formula:");
            if (crossSheetArea.SheetNames != null)
            {
                foreach (string sheetName in crossSheetArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // Spara arbetsboken
            workbook.Save("ReferredAreaSheetNamesDemo.xlsx");
        }
    }
}
```

### Se även

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


