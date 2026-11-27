---
title: "Workbook.HasCustomFunction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Detekterar om det finns en anpassad funktion som används i denna arbetsbok, t.ex. i cellers formel i definierade namn"
type: docs
url: /sv/net/aspose.cells/workbook/hascustomfunction/
---
## Workbook.HasCustomFunction property

Detekterar om det finns anpassade funktioner som används i den här arbetsboken, till exempel i cellers formel eller i definierade namn...

```csharp
public bool HasCustomFunction { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Lägg till en standardformel till ett namn
            NameCollection names = wb.Worksheets.Names;
            int index = names.Add("StandardName");
            names[index].RefersTo = "=SUM(Sheet1!$A$1:$A$2)";
            Console.WriteLine($"Workbook has custom function (should be false): {wb.HasCustomFunction}");

            // Lägg till en anpassad funktion till ett namn
            index = names.Add("CustomName");
            names[index].RefersTo = "=MYFUNC()";
            Console.WriteLine($"Workbook has custom function (should be true): {wb.HasCustomFunction}");

            // Testa med cellformler
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Standardfunktion i cell
            cells["A1"].Formula = "=SUM(B1:B2)";
            Console.WriteLine($"Cell has custom function (should be false): {cells["A1"].HasCustomFunction}");

            // Anpassad funktion i cell
            cells["A2"].Formula = "=MYFUNC(B1)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A2"].HasCustomFunction}");

            // Referens till namn med anpassad funktion
            cells["A3"].Formula = "=CustomName";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A3"].HasCustomFunction}");

            // Kombinerade anpassade funktioner
            cells["A4"].Formula = "=MYFUNC(CustomName)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A4"].HasCustomFunction}");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


