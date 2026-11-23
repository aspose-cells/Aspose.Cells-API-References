---
title: "CustomDocumentPropertyCollection.AddLinkToContent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CustomDocumentPropertyCollection. Crée une nouvelle propriété de document personnalisée qui se lie au contenu"
type: docs
url: /fr/net/aspose.cells.properties/customdocumentpropertycollection/addlinktocontent/
---
## CustomDocumentPropertyCollection.AddLinkToContent method

Crée une nouvelle propriété de document personnalisée qui lie au contenu.

```csharp
public DocumentProperty AddLinkToContent(string name, string source)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la propriété. |
| source | String | La source de la propriété. Elle doit être le nom de la plage nommée. |

### Valeur de retour

Le nouvel objet de propriété créé.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddLinkToContentWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir une valeur dans la cellule A1 qui sera liée
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Ajouter une propriété régulière pour comparaison
            customProperties.Add("RegularProperty", "Static Value");
            
            // Ajouter une propriété liée
            customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");
            
            // Mettre à jour la valeur liée
            customProperties.UpdateLinkedRange();

            // Afficher les propriétés
            Console.WriteLine($"Regular Property: {customProperties["RegularProperty"].Value}");
            Console.WriteLine($"Linked Property: {customProperties["LinkedProperty"].Value}");

            workbook.Save("LinkedPropertyExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


