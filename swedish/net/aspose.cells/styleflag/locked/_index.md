---
title: "StyleFlag.Locked"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag property. Låst-inställning kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/locked/
---
## StyleFlag.Locked property

Inställning för låst kommer att tillämpas.

```csharp
public bool Locked { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLockedDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa en stil och sätt dess låsta egenskap
            Style style = workbook.CreateStyle();
            style.IsLocked = true;

            // Skapa stilflagga och aktivera låst-flaggan
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Locked = true;

            // Applicera stilen på cell A1
            Cell cell = cells["A1"];
            cell.SetStyle(style, styleFlag);

            // Verifiera den låsta statusen
            Console.WriteLine("Cell A1 is locked: " + cell.GetStyle().IsLocked);

            // Skydda kalkylbladet för att se låseffekten
            worksheet.Protect(ProtectionType.All);

            // Försök att ändra den låsta cellen (kommer att kasta ett undantag när kalkylbladet är skyddat)
            try
            {
                cell.PutValue("Test");
                Console.WriteLine("Cell modified successfully (worksheet not properly protected)");
            }
            catch
            {
                Console.WriteLine("Could not modify locked cell (worksheet protected)");
            }
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


