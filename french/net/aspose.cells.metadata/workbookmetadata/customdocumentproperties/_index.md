---
title: "WorkbookMetadata.CustomDocumentProperties"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookMetadata. Retourne une collection DocumentProperty qui représente toutes les propriétés de document personnalisées de la feuille de calcul."
type: docs
url: /fr/net/aspose.cells.metadata/workbookmetadata/customdocumentproperties/
---
## WorkbookMetadata.CustomDocumentProperties property

Retourne une collection [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) qui représente toutes les propriétés de document personnalisées de la feuille de calcul.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Exemples

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
            // Chemins source et destination.
            string sourcePath = "example.xlsx";
            string destPath = "output.xlsx";

            // Créer des options de métadonnées pour les propriétés du document.
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // Initialiser les métadonnées du classeur.
            WorkbookMetadata meta = new WorkbookMetadata(sourcePath, options);
            
            // Ajouter une propriété de document personnalisée
            meta.CustomDocumentProperties.Add("Author", "John Doe");
            
            // Enregistrer le classeur avec les métadonnées
            meta.Save(destPath);
            
            // Vérifier la propriété personnalisée
            Workbook workbook = new Workbook(destPath);
            Console.WriteLine("Custom Property Value: " + 
                workbook.CustomDocumentProperties["Author"].Value);
        }
    }
}
```

### Voir aussi

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


