---
title: "XlsbSaveOptions.ExportAllColumnIndexes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XlsbSaveOptions-Eigenschaft. Gibt an, ob alle Spaltenindizes für Zellen exportiert werden"
type: docs
url: /de/net/aspose.cells/xlsbsaveoptions/exportallcolumnindexes/
---
## XlsbSaveOptions.ExportAllColumnIndexes property

Gibt an, ob alle Spaltenindizes für Zellen exportiert werden.

```csharp
public bool ExportAllColumnIndexes { get; set; }
```

### Hinweise

Der Standardwert ist true.

### Beispiele

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
            
            // Einige Daten befüllen
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

### Siehe auch

* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


