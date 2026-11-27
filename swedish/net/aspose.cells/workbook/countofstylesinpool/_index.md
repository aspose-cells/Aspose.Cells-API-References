---
title: "Workbook.CountOfStylesInPool"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Hämtar antalet stilar i stilpoolen"
type: docs
url: /sv/net/aspose.cells/workbook/countofstylesinpool/
---
## Workbook.CountOfStylesInPool property

Hämtar antalet stilar i stilpoolen.

```csharp
public int CountOfStylesInPool { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCountOfStylesInPoolDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Hämta initialt antal stilar i poolen
            int initialStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Initial styles in pool: {initialStyleCount}");

            // Lägg till några stilar genom att ändra celler
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Stil 1
            Style style1 = wb.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            cells["A1"].SetStyle(style1);
            
            // Stil 2
            Style style2 = wb.CreateStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            style2.Pattern = BackgroundType.Solid;
            cells["B1"].SetStyle(style2);

            // Hämta uppdaterat antal stilar
            int updatedStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Styles after modifications: {updatedStyleCount}");

            // Spara för att demonstrera stilens beständighet
            wb.Save("output.html", SaveFormat.Html);
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


