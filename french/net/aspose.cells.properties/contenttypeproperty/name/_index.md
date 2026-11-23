---
title: "ContentTypeProperty.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ContentTypeProperty. Retourne ou définit le nom de l'objet"
type: docs
url: /fr/net/aspose.cells.properties/contenttypeproperty/name/
---
## ContentTypeProperty.Name property

Renvoie ou définit le nom de l'objet.

```csharp
public string Name { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une propriété de type de contenu avec le nom "ss"
            workbook.ContentTypeProperties.Add("ss", "bb", "text");
            
            // Enregistrer au format XLS
            workbook.Save("example.xls");
            
            // Recharger le classeur et vérifier la propriété Name
            workbook = new Workbook("example.xls");
            Console.WriteLine("Name property in XLS: " + workbook.ContentTypeProperties[0].Name);
            
            // Enregistrer au format XLSX
            workbook.Save("example.xlsx");
            
            // Recharger et vérifier à nouveau
            workbook = new Workbook("example.xlsx");
            Console.WriteLine("Name property in XLSX: " + workbook.ContentTypeProperties[0].Name);
        }
    }
}
```

### Voir aussi

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


