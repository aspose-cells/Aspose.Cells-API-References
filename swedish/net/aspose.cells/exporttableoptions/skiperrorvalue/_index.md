---
title: "ExportTableOptions.SkipErrorValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportTableOptions egenskap. Anger om ogiltigt värde för kolumnen ska hoppas över. Till exempel om kolumntypen är decimal och värdet är större än decimal.MaxValue och denna egenskap är true kommer vi inte kasta undantag igen. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/exporttableoptions/skiperrorvalue/
---
## ExportTableOptions.SkipErrorValue property

Indikerar om ogiltiga värden för kolumnen ska hoppas över. Till exempel, om kolumntypen är decimal, värdet är större än decimal.MaxValue och denna egenskap är true, kommer vi inte att kasta ett undantag igen. Standardvärdet är false.

```csharp
public bool SkipErrorValue { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertySkipErrorValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;

            Worksheet ws = wb.Worksheets[0];

            // Första testfallet - numeriska värden
            ws.Cells["A1"].Value = "Double";
            ws.Cells["A2"].Value = 1.56;

            ExportTableOptions eto = new ExportTableOptions();
            eto.ExportColumnName = true;
            eto.SkipErrorValue = true;
            eto.CheckMixedValueType = true;

            DataTable data = ws.Cells.ExportDataTable(0, 0, 2, 1, eto);
            Console.WriteLine("Is string: " + (data.Rows[0][0] is string)); // Should be False
            Console.WriteLine("Value: " + data.Rows[0][0]); // Should be 1.56

            // Andra testfallet - blandade värden
            ws.Cells["A2"].Value = "dummy";
            ws.Cells["A3"].Value = 1.56;

            data = ws.Cells.ExportDataTable(0, 0, 3, 1, eto);
            Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
            Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"

            // Tredje testfallet - exportera som sträng
            data = ws.Cells.ExportDataTableAsString(0, 0, 3, 1, true);
            Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
            Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"
        }
    }
}
```

### Se även

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


