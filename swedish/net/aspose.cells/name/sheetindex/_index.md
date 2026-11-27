---
title: "Name.SheetIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Name-egenskap. Anger att detta namn tillhör Workbook eller Worksheet. 0 Globalt namn annars index till bladet enbaserat"
type: docs
url: /sv/net/aspose.cells/name/sheetindex/
---
## Name.SheetIndex property

Anger att detta namn tillhör Workbook eller Worksheet. 0 = Globalt namn, annars index till blad (en‑baserat)

```csharp
public int SheetIndex { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertySheetIndexDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till några arbetsblad
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Skapa ett namngivet område i Sheet2
            Worksheet sheet2 = workbook.Worksheets["Sheet2"];
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet2!$A$1:$B$10";
            
            // Visa bladindexet för det namngivna området
            Console.WriteLine("Sheet index of named range: " + name.SheetIndex);
            
            // Spara arbetsboken
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


