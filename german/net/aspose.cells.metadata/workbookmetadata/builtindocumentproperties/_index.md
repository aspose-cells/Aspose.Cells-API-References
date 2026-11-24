---
title: "WorkbookMetadata.BuiltInDocumentProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookMetadata-Eigenschaft. Gibt eine DocumentProperty-Sammlung zurück, die alle integrierten Dokumenteigenschaften der Tabelle darstellt"
type: docs
url: /de/net/aspose.cells.metadata/workbookmetadata/builtindocumentproperties/
---
## WorkbookMetadata.BuiltInDocumentProperties property

Gibt eine [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/)‑Sammlung zurück, die alle integrierten Dokumenteigenschaften der Tabelle darstellt.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Speichere die Arbeitsmappe in einer Datei
                string filePath = "BuiltInDocumentPropertiesDemo.xlsx";
                workbook.Save(filePath);

                // Erstelle Metadatenoptionen für Dokumenteigenschaften
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // Initialisiere Arbeitsmappen-Metadaten
                WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

                // Greife auf integrierte Dokumenteigenschaften zu (schreibgeschützt)
                var builtInProps = metadata.BuiltInDocumentProperties;

                // Zeige einige integrierte Dokumenteigenschaften an
                Console.WriteLine("Built-in Document Properties:");
                Console.WriteLine("Author: " + builtInProps.Author);
                Console.WriteLine("Title: " + builtInProps.Title);
                Console.WriteLine("Subject: " + builtInProps.Subject);
                Console.WriteLine("Created Time: " + builtInProps.CreatedTime);
                Console.WriteLine("Last Saved By: " + builtInProps.LastSavedBy);
                Console.WriteLine("Total Editing Time: " + builtInProps.TotalEditingTime);

                // Ändere einige integrierte Eigenschaften (da sie les- und schreibbar sind)
                builtInProps.Author = "Aspose Developer";
                builtInProps.Title = "BuiltIn Properties Demo";
                builtInProps.Subject = "Demonstrating BuiltInDocumentProperties";
                builtInProps.Company = "Aspose";
                builtInProps.Comments = "This demonstrates the BuiltInDocumentProperties API";

                // Speichere die Metadatenänderungen
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

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


