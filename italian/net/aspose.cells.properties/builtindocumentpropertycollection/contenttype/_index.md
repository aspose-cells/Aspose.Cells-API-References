---
title: "BuiltInDocumentPropertyCollection.ContentType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta il tipo di contenuto del documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/contenttype/
---
## BuiltInDocumentPropertyCollection.ContentType property

Ottiene o imposta il tipo di contenuto del documento.

```csharp
public string ContentType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyContentTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Imposta la proprietà ContentType
            workbook.BuiltInDocumentProperties.ContentType = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet";

            // Visualizza la proprietà ContentType
            Console.WriteLine("ContentType: " + workbook.BuiltInDocumentProperties.ContentType);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


