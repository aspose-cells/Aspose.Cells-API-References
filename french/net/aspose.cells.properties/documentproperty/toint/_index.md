---
title: "DocumentProperty.ToInt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode DocumentProperty. Retourne la valeur de la propriété en tant qu'entier"
type: docs
url: /fr/net/aspose.cells.properties/documentproperty/toint/
---
## DocumentProperty.ToInt method

Renvoie la valeur de la propriété en tant qu'entier.

```csharp
public int ToInt()
```

### Remarques

Lance une exception si le type de la propriété n'est pas PropertyType.Number.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToIntDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Obtenir la collection des propriétés de document personnalisées
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Ajouter une propriété personnalisée numérique
            customProperties.Add("Revision", 5);

            // Obtenez la propriété et convertissez‑la en int en utilisant ToInt()
            DocumentProperty revisionProperty = customProperties["Revision"];
            int revisionValue = revisionProperty.ToInt();
            
            // Afficher le résultat
            Console.WriteLine($"Revision (as int): {revisionValue}");

            // Enregistrez le classeur
            workbook.Save("DocumentPropertyToIntExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


