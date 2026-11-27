---
title: "ReferredArea.StartColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReferredArea-egenskap. Startkolumnen för området"
type: docs
url: /sv/net/aspose.cells/referredarea/startcolumn/
---
## ReferredArea.StartColumn property

Startkolumnen för området.

```csharp
public int StartColumn { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyStartColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["B1"].PutValue("Banana");
            worksheet.Cells["C1"].PutValue("Cherry");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].PutValue(30);

            // Skapa ett namngivet område som refererar till B1:C2
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!B1:C2";

            // Hämta det refererade området med recalculate satt till false
            ReferredArea referredArea = name.GetReferredAreas(false)[0];

            // Demonstrera StartColumn-egenskapen
            Console.WriteLine("Start Column: " + referredArea.StartColumn);
            Console.WriteLine("End Column: " + referredArea.EndColumn);

            // Skriv ut värden i det refererade området med hjälp av StartColumn
            Cells cells = worksheet.Cells;
            for (int row = referredArea.StartRow; row <= referredArea.EndRow; row++)
            {
                for (int col = referredArea.StartColumn; col <= referredArea.EndColumn; col++)
                {
                    Console.WriteLine(cells[row, col].Name + ": " + cells[row, col].Value);
                }
            }
        }
    }
}
```

### Se även

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


