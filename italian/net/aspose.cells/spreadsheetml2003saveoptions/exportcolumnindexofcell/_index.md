---
title: "SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SpreadsheetML2003SaveOptions. Il valore predefinito è false, il che significa che l'indice di colonna sarà ignorato se la cella è contigua alla cella precedente."
type: docs
url: /it/net/aspose.cells/spreadsheetml2003saveoptions/exportcolumnindexofcell/
---
## SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell property

Il valore predefinito è false, significa che l'indice della colonna verrà ignorato se la cella è contigua alla cella precedente.

```csharp
public bool ExportColumnIndexOfCell { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyExportColumnIndexOfCellDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            
            // Crea le opzioni di salvataggio con ExportColumnIndexOfCell abilitato
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.ExportColumnIndexOfCell = true;
            
            // Salva la cartella di lavoro con le informazioni sull'indice di colonna
            workbook.Save("output_with_column_index.xml", saveOptions);
            
            Console.WriteLine("File saved with column index information.");
        }
    }
}
```

### Vedi anche

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


