---
title: "WorkbookMetadata.BuiltInDocumentProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookMetadata. Restituisce una raccolta DocumentProperty che rappresenta tutte le proprietà documento integrate del foglio di calcolo"
type: docs
url: /it/net/aspose.cells.metadata/workbookmetadata/builtindocumentproperties/
---
## WorkbookMetadata.BuiltInDocumentProperties property

Restituisce una raccolta [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) che rappresenta tutte le proprietà di documento incorporate del foglio di calcolo.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class WorkbookMetadataPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Salva la cartella di lavoro in un file
                string filePath = "BuiltInDocumentPropertiesDemo.xlsx";
                workbook.Save(filePath);

                // Crea opzioni di metadati per le proprietà del documento
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // Inizializza i metadati della cartella di lavoro
                WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

                // Accedi alle proprietà documento integrate (sola lettura)
                var builtInProps = metadata.BuiltInDocumentProperties;

                // Visualizza alcune proprietà documento integrate
                Console.WriteLine("Built-in Document Properties:");
                Console.WriteLine("Author: " + builtInProps.Author);
                Console.WriteLine("Title: " + builtInProps.Title);
                Console.WriteLine("Subject: " + builtInProps.Subject);
                Console.WriteLine("Created Time: " + builtInProps.CreatedTime);
                Console.WriteLine("Last Saved By: " + builtInProps.LastSavedBy);
                Console.WriteLine("Total Editing Time: " + builtInProps.TotalEditingTime);

                // Modifica alcune proprietà integrate (poiché sono leggibili e scrivibili)
                builtInProps.Author = "Aspose Developer";
                builtInProps.Title = "BuiltIn Properties Demo";
                builtInProps.Subject = "Demonstrating BuiltInDocumentProperties";
                builtInProps.Company = "Aspose";
                builtInProps.Comments = "This demonstrates the BuiltInDocumentProperties API";

                // Salva le modifiche ai metadati
                metadata.Save(filePath);

                Console.WriteLine("\nBuilt-in properties have been updated and saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


