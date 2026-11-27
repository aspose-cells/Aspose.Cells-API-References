---
title: "TxtLoadOptions.MaxRowCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtLoadOptions-egenskap. Det maximala antalet rader som ska importeras för ett blad"
type: docs
url: /sv/net/aspose.cells/txtloadoptions/maxrowcount/
---
## TxtLoadOptions.MaxRowCount property

Det maximala antalet rader som ska importeras för ett blad.

```csharp
public int MaxRowCount { get; set; }
```

### Anmärkningar

Rader som överskrider denna gräns kommer att ignoreras eller utökas till nästa blad enligt [`ExtendToNextSheet`](../extendtonextsheet/). Detta antal inkluderar rubrikraderna([`HeaderRowsCount`](../headerrowscount/)). Det högsta tillåtna värdet är radgränsen för motsvarande filformat, till exempel för xlsx-filen är den 1048576. Om denna egenskap inte har angetts eller det angivna värdet inte är positivt, används det maximala gränsvärdet också.

### Exempel

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyMaxRowCountDemo
    {
        public static void Run()
        {
            // Skapa exempel-CSV-innehåll
            string content = "Header1,Header2,Header3\n" +
                            "Data1,Data2,Data3\n" +
                            "Data4,Data5,Data6\n" +
                            "Data7,Data8,Data9\n" +
                            "Data10,Data11,Data12\n" +
                            "Data13,Data14,Data15\n" +
                            "Data16,Data17,Data18";

            // Skapa TxtLoadOptions med MaxRowCount satt till 4
            TxtLoadOptions opts = new TxtLoadOptions
            {
                MaxRowCount = 4,  // Only load first 4 rows (including header)
                HeaderRowsCount = 1  // First row is header
            };

            // Läs in CSV i arbetsboken
            using (MemoryStream ms = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook wb = new Workbook(ms, opts);

                // Verifiera att endast 4 rader lästes in (1 rubrik + 3 datarader)
                Worksheet sheet = wb.Worksheets[0];
                Console.WriteLine($"Total rows loaded: {sheet.Cells.MaxDataRow + 1}");
                Console.WriteLine($"Row 1 (Header): {sheet.Cells[0, 0].StringValue}");
                Console.WriteLine($"Row 2 (Data): {sheet.Cells[1, 0].StringValue}");
                Console.WriteLine($"Row 3 (Data): {sheet.Cells[2, 0].StringValue}");
                Console.WriteLine($"Row 4 (Data): {sheet.Cells[3, 0].StringValue}");

                // Detta skulle vara null eftersom vi bara läste in 4 rader (index 0-3)
                if (sheet.Cells[4, 0] == null || string.IsNullOrEmpty(sheet.Cells[4, 0].StringValue))
                {
                    Console.WriteLine("Row 5 was not loaded due to MaxRowCount limitation");
                }
            }
        }
    }
}
```

### Se även

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


