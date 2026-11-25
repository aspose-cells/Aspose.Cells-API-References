---
title: "WorkbookMetadata.CustomDocumentProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookMetadata. Restituisce una collezione DocumentProperty che rappresenta tutte le proprietà personalizzate del documento del foglio di calcolo"
type: docs
url: /it/net/aspose.cells.metadata/workbookmetadata/customdocumentproperties/
---
## WorkbookMetadata.CustomDocumentProperties property

Restituisce una raccolta di [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) che rappresenta tutte le proprietà personalizzate del documento del foglio di calcolo.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Percorsi di origine e destinazione
            string sourcePath = "example.xlsx";
            string destPath = "output.xlsx";

            // Crea opzioni di metadati per le proprietà del documento
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // Inizializza i metadati della cartella di lavoro
            WorkbookMetadata meta = new WorkbookMetadata(sourcePath, options);
            
            // Aggiungi proprietà documento personalizzata
            meta.CustomDocumentProperties.Add("Author", "John Doe");
            
            // Salva la cartella di lavoro con i metadati
            meta.Save(destPath);
            
            // Verifica la proprietà personalizzata
            Workbook workbook = new Workbook(destPath);
            Console.WriteLine("Custom Property Value: " + 
                workbook.CustomDocumentProperties["Author"].Value);
        }
    }
}
```

### Vedi anche

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


