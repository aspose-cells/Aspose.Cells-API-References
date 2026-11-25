---
title: "BuiltInDocumentPropertyCollection.Language"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "BuiltInDocumentPropertyCollection property. Ottiene o imposta la lingua del documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/language/
---
## BuiltInDocumentPropertyCollection.Language property

Ottiene o imposta la lingua del documento.

```csharp
public string Language { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLanguageDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alla collezione delle proprietà del documento integrate
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Imposta la proprietà language
            builtInProperties.Language = "en-US";

            // Imposta altre proprietà di base per la dimostrazione
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Language Property Demo";

            // Salva la cartella di lavoro
            workbook.Save("LanguagePropertyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


