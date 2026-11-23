---
title: "CustomDocumentPropertyCollection.UpdateLinkedRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "CustomDocumentPropertyCollection method. Met à jour toutes les plages qui sont liées aux propriétés personnalisées en utilisant la valeur de la propriété de document personnalisée pour mettre à jour la valeur de la cellule de la plage liée"
type: docs
url: /fr/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange/
---
## CustomDocumentPropertyCollection.UpdateLinkedRange method

Met à jour toutes les plages qui sont liées aux propriétés personnalisées (utilise la valeur de la propriété de document personnalisée pour mettre à jour la valeur de cellule de la plage liée).

```csharp
public void UpdateLinkedRange()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir une valeur dans la cellule A1 qui sera liée
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Ajouter une propriété liée
            customProperties.AddLinkToContent("LinkedRange", "Sheet1!A1");
            
            // Mettre à jour toutes les propriétés liées
            customProperties.UpdateLinkedRange();
            
            // Obtenir et afficher la valeur de la propriété liée
            DocumentProperty linkedProp = customProperties["LinkedRange"];
            Console.WriteLine($"Linked Property Value: {linkedProp.Value}");

            // Enregistrez le classeur
            workbook.Save("LinkedRangeExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


