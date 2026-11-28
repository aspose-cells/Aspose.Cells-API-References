---
title: "CustomPropertyCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomPropertyCollection yöntemi. Özel özellik bilgisi ekler"
type: docs
url: /tr/net/aspose.cells.properties/custompropertycollection/add/
---
## CustomPropertyCollection.Add method

Özel özellik bilgisi ekler.

```csharp
public int Add(string name, string value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Özel özelliğin adı. |
| değer | String | Özel özelliğin değeri. |

### Örnekler

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

### Ayrıca Bakınız

* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


