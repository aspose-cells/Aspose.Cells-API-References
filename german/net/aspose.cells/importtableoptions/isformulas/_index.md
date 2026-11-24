---
title: "ImportTableOptions.IsFormulas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImportTableOptions-Eigenschaft. Gibt an, ob die Daten Formeln sind"
type: docs
url: /de/net/aspose.cells/importtableoptions/isformulas/
---
## ImportTableOptions.IsFormulas property

Gibt an, ob die Daten Formeln sind.

```csharp
public bool[] IsFormulas { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstellen Sie eine Beispieldatentabelle mit Formelinhalten
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1");
            dt.Rows.Add("=SUM(1,2,3)");
            dt.Rows.Add("=AVERAGE(4,5,6)");

            // Importoptionen mit der Eigenschaft IsFormulas festlegen
            ImportTableOptions options = new ImportTableOptions();
            options.IsFormulas = new bool[] { true }; // Treat first column as formulas
            
            // Daten mit Formeln importieren
            workbook.Worksheets[0].Cells.ImportData(dt, 0, 0, options);

            // Überprüfen, ob die Formeln korrekt importiert wurden
            Console.WriteLine("Cell A1 formula: " + workbook.Worksheets[0].Cells["A1"].Formula);
            Console.WriteLine("Cell A2 formula: " + workbook.Worksheets[0].Cells["A2"].Formula);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


