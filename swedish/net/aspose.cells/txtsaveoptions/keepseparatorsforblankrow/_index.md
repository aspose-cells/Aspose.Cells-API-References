---
title: "TxtSaveOptions.KeepSeparatorsForBlankRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtSaveOptions-egenskap. Anger om separatorer ska skrivas ut för tom rad. Standardvärdet är false så innehållet för tom rad blir tomt som standard."
type: docs
url: /sv/net/aspose.cells/txtsaveoptions/keepseparatorsforblankrow/
---
## TxtSaveOptions.KeepSeparatorsForBlankRow property

Anger om avgränsare ska skrivas ut för tom rad. Standardvärdet är falskt, så som standard blir innehållet för en tom rad tomt.

```csharp
public bool KeepSeparatorsForBlankRow { get; set; }
```

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyKeepSeparatorsForBlankRowDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Lägg till lite data med tomma rader
            cells[0, 0].PutValue("a");
            cells[0, 1].PutValue("b");
            cells[3, 0].PutValue("c");
            cells[4, 1].PutValue("d");

            // Skapa sparalternativ med KeepSeparatorsForBlankRow satt till true
            TxtSaveOptions options = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                KeepSeparatorsForBlankRow = true
            };

            // Spara arbetsboken till CSV med alternativen
            string csvOutput = SaveAsCsv(wb, options);
            Console.WriteLine(csvOutput);
        }

        private static string SaveAsCsv(Workbook wb, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                wb.Save(stream, options);
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


