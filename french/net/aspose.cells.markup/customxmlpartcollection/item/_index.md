---
title: "CustomXmlPartCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CustomXmlPartCollection. Obtient un élément à l'index spécifié"
type: docs
url: /fr/net/aspose.cells.markup/customxmlpartcollection/item/
---
## CustomXmlPartCollection indexer

Obtient un élément à l'index spécifié.

```csharp
public CustomXmlPart this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class CustomXmlPartCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder au CustomXmlPartCollection directement depuis le classeur
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // Exemple de données XML
            string xmlData = "<root><item>Test Data</item></root>";
            byte[] xmlBytes = System.Text.Encoding.UTF8.GetBytes(xmlData);
            
            // Ajouter une partie XML personnalisée
            int index = customXmlParts.Add(xmlBytes, null);
            
            // Accéder à l'élément en utilisant la propriété Item
            CustomXmlPart part = customXmlParts[index];
            
            // Afficher l'ID de la partie XML personnalisée
            Console.WriteLine("Custom XML Part ID: " + part.ID);
            
            // Récupérer les données XML de la partie
            string retrievedXml = System.Text.Encoding.UTF8.GetString(part.Data);
            Console.WriteLine("XML Content: " + retrievedXml);
            
            // Enregistrez le classeur
            workbook.Save("CustomXmlPartDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CustomXmlPart](../../customxmlpart/)
* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


