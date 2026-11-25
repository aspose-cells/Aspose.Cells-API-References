---
title: "XlsbSaveOptions.ExportAllColumnIndexes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XlsbSaveOptions. Indica se esportare tutti gli indici di colonna per le celle"
type: docs
url: /it/net/aspose.cells/xlsbsaveoptions/exportallcolumnindexes/
---
## XlsbSaveOptions.ExportAllColumnIndexes property

Indica se esportare tutti gli indici di colonna per le celle.

```csharp
public bool ExportAllColumnIndexes { get; set; }
```

### Osservazioni

Il valore predefinito è true.

### Esempi

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
            
            // Popola alcuni dati
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

### Vedi anche

* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


