---
title: "CustomPropertyCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "CustomPropertyCollection méthode. Ajoute des informations de propriété personnalisée"
type: docs
url: /fr/net/aspose.cells.properties/custompropertycollection/add/
---
## CustomPropertyCollection.Add method

Ajoute des informations de propriété personnalisée.

```csharp
public int Add(string name, string value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la propriété personnalisée. |
| valeur | String | La valeur de la propriété personnalisée. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomPropertyCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CustomPropertyCollection customProperties = worksheet.CustomProperties;
            
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");

            foreach (CustomProperty property in customProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            workbook.Save("CustomPropertiesExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


