---
title: "DocumentProperty.ToDouble"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode DocumentProperty. Retourne la valeur de la propriété en tant que double"
type: docs
url: /fr/net/aspose.cells.properties/documentproperty/todouble/
---
## DocumentProperty.ToDouble method

Renvoie la valeur de la propriété en tant que double.

```csharp
public double ToDouble()
```

### Remarques

Lance une exception si le type de propriété n'est pas PropertyType.Float.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDoubleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Obtenez la collection des propriétés de document personnalisées
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Ajouter une propriété numérique
            customProperties.Add("Rating", 4.75);

            // Obtenir la propriété et la convertir en double
            DocumentProperty ratingProperty = customProperties["Rating"];
            double ratingValue = ratingProperty.ToDouble();

            // Afficher le résultat
            Console.WriteLine($"Rating: {ratingValue}");

            // Enregistrez le classeur
            workbook.Save("DocumentPropertyToDoubleExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


