---
title: "SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Eigenschaft SpreadsheetML2003SaveOptions. Der Standardwert ist false, das bedeutet, dass der Spaltenindex ignoriert wird, wenn die Zelle an die vorherige Zelle angrenzt."
type: docs
url: /de/net/aspose.cells/spreadsheetml2003saveoptions/exportcolumnindexofcell/
---
## SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell property

Der Standardwert ist false, das bedeutet, dass der Spaltenindex ignoriert wird, wenn die Zelle an die vorherige Zelle angrenzt.

```csharp
public bool ExportColumnIndexOfCell { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyExportColumnIndexOfCellDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            
            // Erstellen Sie Speicheroptionen mit aktiviertem ExportColumnIndexOfCell
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.ExportColumnIndexOfCell = true;
            
            // Speichern Sie die Arbeitsmappe mit Spaltenindexinformationen
            workbook.Save("output_with_column_index.xml", saveOptions);
            
            Console.WriteLine("File saved with column index information.");
        }
    }
}
```

### Siehe auch

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


