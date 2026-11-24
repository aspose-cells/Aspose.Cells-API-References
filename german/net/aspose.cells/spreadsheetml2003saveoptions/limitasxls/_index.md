---
title: "SpreadsheetML2003SaveOptions.LimitAsXls"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Eigenschaft SpreadsheetML2003SaveOptions. Limit als xls: Der maximale Zeilenindex ist 65535 und der maximale Spaltenindex ist 255"
type: docs
url: /de/net/aspose.cells/spreadsheetml2003saveoptions/limitasxls/
---
## SpreadsheetML2003SaveOptions.LimitAsXls property

Begrenzung für xls: Der maximale Zeilenindex ist 65535 und der maximale Spaltenindex ist 255.

```csharp
public bool LimitAsXls { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyLimitAsXlsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // Greifen Sie auf Zellen zu und erstellen Sie einen Bereich
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "C5");
            range.Name = "TestRange";
            
            // Speichern mit LimitAsXls = true
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions()
            {
                LimitAsXls = true
            };
            
            // Speichern als SpreadsheetML mit XLS-Begrenzungen
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with LimitAsXls=true");
        }
    }
}
```

### Siehe auch

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


