---
title: "Name.Text"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Name-egenskap. Hämtar namntexten för objektet"
type: docs
url: /sv/net/aspose.cells/name/text/
---
## Name.Text property

Hämtar namntexten för objektet.

```csharp
public string Text { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyTextDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett namngivet område
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
            
            // Ställ in och visa Text-egenskapen
            namedRange.Text = "MyCustomName";
            Console.WriteLine("Named range text: " + namedRange.Text);
            
            // Spara arbetsboken
            workbook.Save("NamedRangeExample.xlsx");
        }
    }
}
```

### Se även

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


