---
title: "CustomPropertyCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CustomPropertyCollection. Aggiunge informazioni sulla proprietà personalizzata"
type: docs
url: /it/net/aspose.cells.properties/custompropertycollection/add/
---
## CustomPropertyCollection.Add method

Aggiunge informazioni sulla proprietà personalizzata.

```csharp
public int Add(string name, string value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della proprietà personalizzata. |
| valore | String | Il valore della proprietà personalizzata. |

### Esempi

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

### Vedi anche

* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


