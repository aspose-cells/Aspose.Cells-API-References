---
title: "SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SpreadsheetML2003SaveOptions egenskap. Standardvärdet är false, det betyder att kolumnindex ignoreras om cellen är sammanhängande med föregående cell"
type: docs
url: /sv/net/aspose.cells/spreadsheetml2003saveoptions/exportcolumnindexofcell/
---
## SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell property

Standardvärdet är false, vilket betyder att kolumnindex ignoreras om cellen är intill den föregående cellen.

```csharp
public bool ExportColumnIndexOfCell { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyExportColumnIndexOfCellDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            
            // Skapa sparalternativ med ExportColumnIndexOfCell aktiverat
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.ExportColumnIndexOfCell = true;
            
            // Spara arbetsboken med kolumnindexinformation
            workbook.Save("output_with_column_index.xml", saveOptions);
            
            Console.WriteLine("File saved with column index information.");
        }
    }
}
```

### Se även

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


