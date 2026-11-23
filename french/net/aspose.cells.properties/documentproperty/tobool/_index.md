---
title: "DocumentProperty.ToBool"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode DocumentProperty. Retourne la valeur de la propriété en tant que bool"
type: docs
url: /fr/net/aspose.cells.properties/documentproperty/tobool/
---
## DocumentProperty.ToBool method

Renvoie la valeur de la propriété en tant que bool.

```csharp
public bool ToBool()
```

### Remarques

Lance une exception si le type de propriété n'est pas PropertyType.Boolean.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToBoolDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Ajouter une propriété personnalisée du document booléenne
            customProperties.Add("IsApproved", true);
            
            // Obtenir la propriété et la convertir en bool en utilisant ToBool()
            DocumentProperty isApprovedProperty = customProperties["IsApproved"];
            bool isApproved = isApprovedProperty.ToBool();
            
            Console.WriteLine($"Is Approved: {isApproved}");
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


