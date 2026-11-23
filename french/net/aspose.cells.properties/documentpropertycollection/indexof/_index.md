---
title: "DocumentPropertyCollection.IndexOf"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode DocumentPropertyCollection. Obtient l'indice d'une propriété par son nom"
type: docs
url: /fr/net/aspose.cells.properties/documentpropertycollection/indexof/
---
## DocumentPropertyCollection.IndexOf method

Obtient l'indice d'une propriété par son nom.

```csharp
public int IndexOf(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la propriété, insensible à la casse. |

### Valeur de retour

L'indice basé sur zéro. Valeur négative si non trouvé.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyCollectionMethodIndexOfWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenir la collection des propriétés de document intégrées
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;

            // Pour les propriétés intégrées, nous ne pouvons définir que les valeurs des propriétés existantes
            // Pour ajouter des propriétés personnalisées, nous devrions utiliser CustomDocumentPropertyCollection
            // Ici, nous allons simplement définir quelques propriétés intégrées existantes à des fins de démonstration
            properties["Title"].Value = "Value1";
            properties["Subject"].Value = "Value2";
            properties["Author"].Value = "Value3";

            try
            {
                // Appelez la méthode IndexOf avec un paramètre de chaîne
                int index = properties.IndexOf("Subject");
                
                // Afficher le résultat
                Console.WriteLine($"Index of 'Subject': {index}");
                
                // Afficher la propriété à l'indice trouvé
                if (index >= 0)
                {
                    DocumentProperty property = properties[index];
                    Console.WriteLine($"Property at index {index}: {property.Name} = {property.Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IndexOf method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("DocumentPropertyIndexOfDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


