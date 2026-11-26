---
title: "CustomPropertyCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CustomPropertyCollection. Añade información de propiedad personalizada"
type: docs
url: /es/net/aspose.cells.properties/custompropertycollection/add/
---
## CustomPropertyCollection.Add method

Agrega información de propiedad personalizada.

```csharp
public int Add(string name, string value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la propiedad personalizada. |
| valor | String | El valor de la propiedad personalizada. |

### Ejemplos

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

### Ver también

* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


