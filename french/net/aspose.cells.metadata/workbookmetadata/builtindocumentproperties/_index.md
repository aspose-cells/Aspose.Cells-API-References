---
title: "WorkbookMetadata.BuiltInDocumentProperties"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookMetadata. Retourne une collection DocumentProperty qui représente toutes les propriétés de document intégrées de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.metadata/workbookmetadata/builtindocumentproperties/
---
## WorkbookMetadata.BuiltInDocumentProperties property

Retourne une collection [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) qui représente toutes les propriétés de document intégrées de la feuille de calcul.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Enregistrer le classeur dans un fichier
                string filePath = "BuiltInDocumentPropertiesDemo.xlsx";
                workbook.Save(filePath);

                // Créer des options de métadonnées pour les propriétés du document.
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // Initialiser les métadonnées du classeur.
                WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

                // Accéder aux propriétés de document intégrées (lecture seule)
                var builtInProps = metadata.BuiltInDocumentProperties;

                // Afficher certaines propriétés de document intégrées
                Console.WriteLine("Built-in Document Properties:");
                Console.WriteLine("Author: " + builtInProps.Author);
                Console.WriteLine("Title: " + builtInProps.Title);
                Console.WriteLine("Subject: " + builtInProps.Subject);
                Console.WriteLine("Created Time: " + builtInProps.CreatedTime);
                Console.WriteLine("Last Saved By: " + builtInProps.LastSavedBy);
                Console.WriteLine("Total Editing Time: " + builtInProps.TotalEditingTime);

                // Modifier certaines propriétés intégrées (car elles sont en lecture-écriture)
                builtInProps.Author = "Aspose Developer";
                builtInProps.Title = "BuiltIn Properties Demo";
                builtInProps.Subject = "Demonstrating BuiltInDocumentProperties";
                builtInProps.Company = "Aspose";
                builtInProps.Comments = "This demonstrates the BuiltInDocumentProperties API";

                // Enregistrer les modifications des métadonnées
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

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


