---
title: "CustomPropertyCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomPropertyCollection Methode. Fügt benutzerdefinierte Property-Informationen hinzu"
type: docs
url: /de/net/aspose.cells.properties/custompropertycollection/add/
---
## CustomPropertyCollection.Add method

Fügt benutzerdefinierte Eigenschaftsinformationen hinzu.

```csharp
public int Add(string name, string value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der benutzerdefinierten Property. |
| Wert | String | Der Wert der benutzerdefinierten Property. |

### Beispiele

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

### Siehe auch

* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


