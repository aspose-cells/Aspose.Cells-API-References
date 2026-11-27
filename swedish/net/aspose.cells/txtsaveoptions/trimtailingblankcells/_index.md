---
title: "TxtSaveOptions.TrimTailingBlankCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtSaveOptions egenskap. Anger om efterföljande tomma celler i en rad ska tas bort. Standard är falskt."
type: docs
url: /sv/net/aspose.cells/txtsaveoptions/trimtailingblankcells/
---
## TxtSaveOptions.TrimTailingBlankCells property

Anger om avslutande tomma celler i en rad ska tas bort. Standard är falskt.

```csharp
public bool TrimTailingBlankCells { get; set; }
```

### Anmärkningar

När du sparar med LightCells-läge och [`ExportArea`](../exportarea/) inte har angetts, har detta alternativ ingen effekt och en rad kommer att utökas till endast den sista cellen som tillhandahålls av implementationen [`LightCellsDataProvider`](../lightcellsdataprovider/).

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyTrimTailingBlankCellsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Lägg till exempeldata
            cells[0, 0].PutValue("A");
            cells[0, 1].PutValue("B");
            cells[0, 2].PutValue("C");
            cells[1, 0].PutValue(1);
            cells[1, 2].PutValue(2);
            cells[2, 0].PutValue(3);

            // Spara utan att ta bort efterföljande tomma celler (standard)
            TxtSaveOptions options1 = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                TrimTailingBlankCells = false
            };
            string result1 = SaveAsCsv(workbook, options1);
            Console.WriteLine("Without TrimTailingBlankCells:\n" + result1);

            // Spara med att ta bort efterföljande tomma celler
            TxtSaveOptions options2 = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                TrimTailingBlankCells = true
            };
            string result2 = SaveAsCsv(workbook, options2);
            Console.WriteLine("\nWith TrimTailingBlankCells:\n" + result2);
        }

        private static string SaveAsCsv(Workbook workbook, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                workbook.Save(stream, options);
                return Encoding.ASCII.GetString(stream.ToArray());
            }
        }
    }
}
```

### Se även

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


