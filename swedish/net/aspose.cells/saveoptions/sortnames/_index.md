---
title: "SaveOptions.SortNames"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SaveOptions-egenskap. Anger om definierade namn ska sorteras innan filen sparas"
type: docs
url: /sv/net/aspose.cells/saveoptions/sortnames/
---
## SaveOptions.SortNames property

Anger om definierade namn ska sorteras innan filen sparas.

```csharp
public bool SortNames { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertySortNamesDemo
    {
        public static void Run()
        {
            // Skapa ett nytt Workbook-objekt
            Workbook workbook = new Workbook();
            
            // Lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Skapa ett namngivet område
            worksheet.Cells.CreateRange("A2:B3").Name = "MyDataRange";

            // Skapa sparalternativ med SortNames aktiverat
            XlsSaveOptions saveOptions = new XlsSaveOptions
            {
                SortNames = true
            };

            // Spara arbetsboken
            workbook.Save("SortedNamesExample.xls", saveOptions);

            Console.WriteLine("Workbook saved with sorted named ranges.");
        }
    }
}
```

### Se även

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


