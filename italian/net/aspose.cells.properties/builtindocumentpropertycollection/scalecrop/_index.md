---
title: "BuiltInDocumentPropertyCollection.ScaleCrop"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Indica la modalità di visualizzazione della miniatura del documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/scalecrop/
---
## BuiltInDocumentPropertyCollection.ScaleCrop property

Indica la modalità di visualizzazione della miniatura del documento.

```csharp
public bool ScaleCrop { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyScaleCropDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle proprietà del documento integrate
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Imposta la proprietà ScaleCrop
            properties.ScaleCrop = true;
            
            // Visualizza il valore della proprietà ScaleCrop
            Console.WriteLine("ScaleCrop property value: " + properties.ScaleCrop);
            
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


