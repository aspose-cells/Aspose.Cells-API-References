---
title: "XmlSaveOptions.ExportArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlSaveOptions. Ottiene o imposta l'intervallo di esportazione"
type: docs
url: /it/net/aspose.cells/xmlsaveoptions/exportarea/
---
## XmlSaveOptions.ExportArea property

Ottiene o imposta l'intervallo di esportazione.

```csharp
public CellArea ExportArea { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserisci dati nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea XmlSaveOptions e imposta ExportArea
            XmlSaveOptions saveOptions = new XmlSaveOptions
            {
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // Salva solo l'area specificata in XML
            workbook.Save("ExportAreaDemo.xml", saveOptions);
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


