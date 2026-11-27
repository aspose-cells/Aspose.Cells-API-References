---
title: "XlsbSaveOptions.ExportAllColumnIndexes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XlsbSaveOptions-egenskap. Anger om alla kolumnindex för celler exporteras"
type: docs
url: /sv/net/aspose.cells/xlsbsaveoptions/exportallcolumnindexes/
---
## XlsbSaveOptions.ExportAllColumnIndexes property

Indikerar om alla kolumnindex exporteras för celler.

```csharp
public bool ExportAllColumnIndexes { get; set; }
```

### Anmärkningar

Standardvärdet är sant.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsPropertyExportAllColumnIndexesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i lite data
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["C2"].PutValue(3);

            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                ExportAllColumnIndexes = true // Demonstrate the property usage
            };

            workbook.Save("XlsbExportAllColumnIndexes.xlsb", saveOptions);
        }
    }
}
```

### Se även

* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


