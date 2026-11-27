---
title: "WorkbookMetadata.BuiltInDocumentProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookMetadata‑egenskap. Returnerar en DocumentProperty‑samling som representerar alla inbyggda dokumentegenskaper i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.metadata/workbookmetadata/builtindocumentproperties/
---
## WorkbookMetadata.BuiltInDocumentProperties property

Returnerar en [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) samling som representerar alla inbyggda dokumentegenskaper i kalkylbladet.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Spara arbetsboken till en fil
                string filePath = "BuiltInDocumentPropertiesDemo.xlsx";
                workbook.Save(filePath);

                // Skapa metadataalternativ för dokumentegenskaper
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // Initiera arbetsbokens metadata
                WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

                // Åtkomst till inbyggda dokumentegenskaper (skrivskyddad)
                var builtInProps = metadata.BuiltInDocumentProperties;

                // Visa vissa inbyggda dokumentegenskaper
                Console.WriteLine("Built-in Document Properties:");
                Console.WriteLine("Author: " + builtInProps.Author);
                Console.WriteLine("Title: " + builtInProps.Title);
                Console.WriteLine("Subject: " + builtInProps.Subject);
                Console.WriteLine("Created Time: " + builtInProps.CreatedTime);
                Console.WriteLine("Last Saved By: " + builtInProps.LastSavedBy);
                Console.WriteLine("Total Editing Time: " + builtInProps.TotalEditingTime);

                // Ändra vissa inbyggda egenskaper (eftersom de är läs‑skriv)
                builtInProps.Author = "Aspose Developer";
                builtInProps.Title = "BuiltIn Properties Demo";
                builtInProps.Subject = "Demonstrating BuiltInDocumentProperties";
                builtInProps.Company = "Aspose";
                builtInProps.Comments = "This demonstrates the BuiltInDocumentProperties API";

                // Spara metadataändringarna
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

### Se även

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


