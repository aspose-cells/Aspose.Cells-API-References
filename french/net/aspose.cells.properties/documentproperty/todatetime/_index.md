---
title: "DocumentProperty.ToDateTime"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode DocumentProperty. Retourne la valeur de la propriété en tant que DateTime dans le fuseau horaire local"
type: docs
url: /fr/net/aspose.cells.properties/documentproperty/todatetime/
---
## DocumentProperty.ToDateTime method

Renvoie la valeur de la propriété en tant que DateTime dans le fuseau horaire local.

```csharp
public DateTime ToDateTime()
```

### Remarques

Lance une exception si le type de propriété n’est pas PropertyType.Date.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDateTimeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Obtenez la collection des propriétés de document personnalisées
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Ajoutez une propriété datetime
            DateTime currentTime = DateTime.Now;
            customProperties.Add("LastModified", currentTime);

            // Obtenez la propriété et convertissez‑la en DateTime
            DocumentProperty lastModifiedProperty = customProperties["LastModified"];
            DateTime retrievedTime = lastModifiedProperty.ToDateTime();

            // Afficher le résultat
            Console.WriteLine($"Stored DateTime: {currentTime}");
            Console.WriteLine($"Retrieved DateTime: {retrievedTime}");

            // Enregistrez le classeur
            workbook.Save("DocumentPropertyDateTimeExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


