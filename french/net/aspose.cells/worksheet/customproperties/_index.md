---
title: "Worksheet.CustomProperties"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient un objet représentant les informations d'identifiant associées à une worksheet"
type: docs
url: /fr/net/aspose.cells/worksheet/customproperties/
---
## Worksheet.CustomProperties property

Obtient un objet représentant les informations d'identifiant associées à une feuille de calcul.

```csharp
public CustomPropertyCollection CustomProperties { get; }
```

### Remarques

Worksheet.CustomProperties fournit un mécanisme privilégié pour stocker des données arbitraires. Il prend en charge les composants de documents tiers hérités, ainsi que les situations nécessitant de manière stricte des parties binaires.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCustomPropertiesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des propriétés personnalisées à la worksheet
            worksheet.CustomProperties.Add("Property1", "Value1");
            worksheet.CustomProperties.Add("Property2", "12345");
            worksheet.CustomProperties.Add("Property3", DateTime.Now.ToString());
            
            // Afficher le nombre de propriétés personnalisées
            Console.WriteLine("Custom Properties Count: " + worksheet.CustomProperties.Count);
            
            // Accéder et afficher les valeurs des propriétés
            foreach (var prop in worksheet.CustomProperties)
            {
                Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}");
            }
            
            // Enregistrez le classeur
            workbook.Save("WorksheetCustomPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [CustomPropertyCollection](../../../aspose.cells.properties/custompropertycollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


