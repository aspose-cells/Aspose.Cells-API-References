---
title: "BuiltInDocumentPropertyCollection.Pages"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Rappresenta una stima del numero di pagine nel documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/pages/
---
## BuiltInDocumentPropertyCollection.Pages property

Rappresenta una stima del numero di pagine nel documento.

```csharp
public int Pages { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyPagesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle proprietà del documento integrate
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Imposta la proprietà Pages
            builtInProperties.Pages = 10;

            // Aggiungi un foglio di lavoro e alcuni dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Page Count Demonstration");
            worksheet.Cells["A2"].PutValue($"This document is set to have {builtInProperties.Pages} pages");

            // Salva la cartella di lavoro
            workbook.Save("DocumentPagesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


