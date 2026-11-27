---
title: "ImportTableOptions.IsFormulas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions egenskap. Anger om data är formler"
type: docs
url: /sv/net/aspose.cells/importtableoptions/isformulas/
---
## ImportTableOptions.IsFormulas property

Anger om data är formler.

```csharp
public bool[] IsFormulas { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyIsFormulasDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa exempeldata-tabell med formelinnehåll
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1");
            dt.Rows.Add("=SUM(1,2,3)");
            dt.Rows.Add("=AVERAGE(4,5,6)");

            // Ställ in importalternativ med IsFormulas-egenskap
            ImportTableOptions options = new ImportTableOptions();
            options.IsFormulas = new bool[] { true }; // Treat first column as formulas
            
            // Importera data med formler
            workbook.Worksheets[0].Cells.ImportData(dt, 0, 0, options);

            // Verifiera att formlerna importerades korrekt
            Console.WriteLine("Cell A1 formula: " + workbook.Worksheets[0].Cells["A1"].Formula);
            Console.WriteLine("Cell A2 formula: " + workbook.Worksheets[0].Cells["A2"].Formula);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


