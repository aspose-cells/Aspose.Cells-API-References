---
title: "ImportTableOptions.ConvertNumericData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions egenskap. Hämtar eller anger ett värde som indikerar om strängvärdet ska konverteras till numeriskt eller datumvärde"
type: docs
url: /sv/net/aspose.cells/importtableoptions/convertnumericdata/
---
## ImportTableOptions.ConvertNumericData property

Hämtar eller anger ett värde som indikerar om strängvärdet ska konverteras till numeriskt eller datumvärde.

```csharp
public bool ConvertNumericData { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa exempel på datatabell med numeriska och strängvärden
            DataTable dt = new DataTable();
            dt.Columns.Add("Numbers");
            dt.Columns.Add("Text");
            dt.Rows.Add("123", "456");
            dt.Rows.Add("ABC", "DEF");

            // Hämta de första kalkylbladets celler
            Cells cells = workbook.Worksheets[0].Cells;

            // Skapa importalternativ med ConvertNumericData satt till true
            ImportTableOptions options = new ImportTableOptions();
            options.ConvertNumericData = true;
            options.IsFieldNameShown = true;

            // Importera data med numerisk konvertering
            cells.ImportData(dt, 0, 0, options);

            // Visa resultat
            Console.WriteLine("A2 (numeric converted): " + cells["A2"].Value + " - Type: " + cells["A2"].Type);
            Console.WriteLine("B2 (string remains): " + cells["B2"].StringValue + " - Type: " + cells["B2"].Type);
        }
    }
}
```

### Se även

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


