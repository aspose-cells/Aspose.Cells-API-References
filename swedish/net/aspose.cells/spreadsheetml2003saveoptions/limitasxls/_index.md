---
title: "SpreadsheetML2003SaveOptions.LimitAsXls"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SpreadsheetML2003SaveOptions egenskap. Begränsa som xls, maximalt radindex är 65535 och maximalt kolumnindex är 255"
type: docs
url: /sv/net/aspose.cells/spreadsheetml2003saveoptions/limitasxls/
---
## SpreadsheetML2003SaveOptions.LimitAsXls property

Begränsning för xls, maximalt radindex är 65535 och maximalt kolumnindex är 255.

```csharp
public bool LimitAsXls { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyLimitAsXlsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // Kom åt celler och skapa ett område
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "C5");
            range.Name = "TestRange";
            
            // Spara med LimitAsXls = true
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions()
            {
                LimitAsXls = true
            };
            
            // Spara som SpreadsheetML med XLS-begränsningar
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with LimitAsXls=true");
        }
    }
}
```

### Se även

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


