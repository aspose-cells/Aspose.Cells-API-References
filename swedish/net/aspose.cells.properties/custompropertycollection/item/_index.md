---
title: "CustomPropertyCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomPropertyCollection-egenskapen. Hämtar den anpassade egenskapen med det specifika indexet"
type: docs
url: /sv/net/aspose.cells.properties/custompropertycollection/item/
---
## CustomPropertyCollection indexer (1 of 2)

Hämtar den anpassade egenskapen med det specifika indexet.

```csharp
public CustomProperty this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

Den anpassade egenskapen

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            CustomPropertyCollection customProperties = sheet.CustomProperties;
            
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");
            customProperties.Add("DateCreated", DateTime.Now.ToString("yyyy-MM-dd"));
            
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Property {i}: {property.Name} = {property.Value}");
            }
            
            workbook.Save("CustomPropertiesDemo.xlsx");
        }
    }
}
```

### Se även

* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## CustomPropertyCollection indexer (2 of 2)

Hämtar den anpassade egenskapen med egenskapsnamnet.

```csharp
public CustomProperty this[string name] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| namn | Egenskapsnamnet. |

### Returvärde

Den anpassade egenskapen

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till anpassade egenskaper
            worksheet.CustomProperties.Add("COR_Report", "Quarterly Report");
            worksheet.CustomProperties.Add("COR_ResultSet", "Sales Data");
            
            // Åtkomst till och visning av anpassade egenskaper med Item property
            Console.WriteLine("COR_Report: " + worksheet.CustomProperties["COR_Report"].Value);
            Console.WriteLine("COR_ResultSet: " + worksheet.CustomProperties["COR_ResultSet"].Value);
            
            // Ändra en anpassad egenskap med Item property
            worksheet.CustomProperties["COR_Report"].Value = "Annual Report";
            Console.WriteLine("Updated COR_Report: " + worksheet.CustomProperties["COR_Report"].Value);
        }
    }
}
```

### Se även

* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


