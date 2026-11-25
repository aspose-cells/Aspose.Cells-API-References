---
title: "ImportTableOptions.IsFormulas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImportTableOptions. Indica se i dati sono formule"
type: docs
url: /it/net/aspose.cells/importtableoptions/isformulas/
---
## ImportTableOptions.IsFormulas property

Indica se i dati sono formule.

```csharp
public bool[] IsFormulas { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Crea una tabella di dati di esempio con contenuto di formula
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1");
            dt.Rows.Add("=SUM(1,2,3)");
            dt.Rows.Add("=AVERAGE(4,5,6)");

            // Imposta le opzioni di importazione con la proprietà IsFormulas
            ImportTableOptions options = new ImportTableOptions();
            options.IsFormulas = new bool[] { true }; // Treat first column as formulas
            
            // Importa dati con formule
            workbook.Worksheets[0].Cells.ImportData(dt, 0, 0, options);

            // Verifica che le formule siano state importate correttamente
            Console.WriteLine("Cell A1 formula: " + workbook.Worksheets[0].Cells["A1"].Formula);
            Console.WriteLine("Cell A2 formula: " + workbook.Worksheets[0].Cells["A2"].Formula);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


