---
title: "Classe WorkbookMetadata"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Metadata.WorkbookMetadata. Représente les métadonnées"
type: docs
url: /fr/net/aspose.cells.metadata/workbookmetadata/
---
## WorkbookMetadata class

Représente les métadonnées.

```csharp
public class WorkbookMetadata
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WorkbookMetadata](workbookmetadata/#constructor)(Stream, MetadataOptions) | Créer l'objet de métadonnées. |
| [WorkbookMetadata](workbookmetadata/#constructor_1)(string, MetadataOptions) | Créer l'objet de métadonnées. |

## Propriétés

| Nom | Description |
| --- | --- |
| [BuiltInDocumentProperties](../../aspose.cells.metadata/workbookmetadata/builtindocumentproperties/) { get; } | Renvoie une collection [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) qui représente toutes les propriétés de document intégrées du classeur. |
| [CustomDocumentProperties](../../aspose.cells.metadata/workbookmetadata/customdocumentproperties/) { get; } | Renvoie une collection [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) qui représente toutes les propriétés de document personnalisées du classeur. |
| [Options](../../aspose.cells.metadata/workbookmetadata/options/) { get; } | Obtient les options des métadonnées. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save)(Stream) | Enregistre les métadonnées modifiées dans le flux. |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save_1)(string) | Enregistre les métadonnées modifiées dans le fichier. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using Aspose.Cells.Properties;
    using System;
    using System.IO;

    public class WorkbookMetadataDemo
    {
        public static void WorkbookMetadataExample()
        {
            // Créer une instance de MetadataOptions
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Créer une instance de WorkbookMetadata avec un nom de fichier et des options
            WorkbookMetadata meta = new WorkbookMetadata("WorkbookMetadataExample_original.xlsx", options);

            // Ajouter une propriété de document personnalisée
            meta.CustomDocumentProperties.Add("test", "test");

            // Enregistrer les métadonnées dans un nouveau fichier
            meta.Save("WorkbookMetadataExample.xlsx");

            // Démontrer l'accès aux propriétés de document intégrées
            BuiltInDocumentPropertyCollection builtInProps = meta.BuiltInDocumentProperties;
            Console.WriteLine("Author: " + builtInProps.Author);
            Console.WriteLine("Title: " + builtInProps.Title);

            // Démontrer l'accès aux propriétés de document personnalisées
            CustomDocumentPropertyCollection customProps = meta.CustomDocumentProperties;
            foreach (DocumentProperty prop in customProps)
            {
                Console.WriteLine("Custom Property - Name: " + prop.Name + ", Value: " + prop.Value);
            }

            // Enregistrer les métadonnées dans un flux
            using (FileStream stream = new FileStream("WorkbookMetadataExample2.xlsx", FileMode.Create, FileAccess.Write))
            {
                meta.Save(stream);
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


