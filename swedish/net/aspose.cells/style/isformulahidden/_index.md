---
title: "Style.IsFormulaHidden"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Anger om formeln ska döljas när arbetsbladet är skyddat"
type: docs
url: /sv/net/aspose.cells/style/isformulahidden/
---
## Style.IsFormulaHidden property

Representerar om formeln kommer att döljas när kalkylbladet är skyddat.

```csharp
public bool IsFormulaHidden { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFormulaHiddenDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa en stil med IsFormulaHidden satt till true
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;
            
            // Tillämpa stilen på en cell
            cells["A1"].SetStyle(style);
            cells["A1"].Formula = "=1+1";

            // Skapa en annan stil med IsFormulaHidden satt till false
            Style style2 = workbook.CreateStyle();
            style2.IsFormulaHidden = false;
            
            // Applicera den andra stilen på en annan cell
            cells["B1"].SetStyle(style2);
            cells["B1"].Formula = "=2+2";

            // Skydda kalkylbladet för att se effekten
            worksheet.Protect(ProtectionType.All, "password", null);

            // Spara arbetsboken
            workbook.Save("IsFormulaHiddenDemo.xlsx");

            Console.WriteLine("Workbook saved with IsFormulaHidden examples.");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


