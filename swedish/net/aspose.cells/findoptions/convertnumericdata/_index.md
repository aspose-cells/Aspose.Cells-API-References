---
title: "FindOptions.ConvertNumericData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FindOptions‑egenskap. Hämtar eller anger ett värde som indikerar om den sökta strängvärdet ska konverteras till numerisk data"
type: docs
url: /sv/net/aspose.cells/findoptions/convertnumericdata/
---
## FindOptions.ConvertNumericData property

Hämtar eller anger ett värde som indikerar om den sökta strängvärdet ska konverteras till numerisk data.

```csharp
public bool ConvertNumericData { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata inklusive numeriska värden som strängar
            worksheet.Cells["A1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("456");
            worksheet.Cells["A3"].PutValue("01/28/2010");

            // Skapa sökalternativ och sätt ConvertNumericData till true
            FindOptions options = new FindOptions();
            options.ConvertNumericData = true;

            // Hitta datumvärdet (lagrat som sträng men konverterat till numeriskt under sökningen)
            Cell foundCell = worksheet.Cells.Find("01/28/2010", null, options);

            // Skriv ut resultatet
            if (foundCell != null)
            {
                Console.WriteLine("Found value at: " + foundCell.Name);
                Console.WriteLine("Cell value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("Value not found");
            }
        }
    }
}
```

### Se även

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


