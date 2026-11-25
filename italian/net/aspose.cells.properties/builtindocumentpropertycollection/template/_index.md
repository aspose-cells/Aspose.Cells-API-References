---
title: "BuiltInDocumentPropertyCollection.Template"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta il nome informativo del modello del documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/template/
---
## BuiltInDocumentPropertyCollection.Template property

Ottiene o imposta il nome informativo del modello di documento.

```csharp
public string Template { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTemplateDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle proprietà del documento integrate
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Imposta la proprietà Template
            builtInProperties.Template = "Standard Template";

            // Imposta altre proprietà di base per la dimostrazione
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Template Property Demo";

            // Salva la cartella di lavoro
            workbook.Save("TemplatePropertyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


