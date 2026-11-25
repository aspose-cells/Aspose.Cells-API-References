---
title: "CustomPropertyCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CustomPropertyCollection. Ottiene la proprietà personalizzata tramite l'indice specifico"
type: docs
url: /it/net/aspose.cells.properties/custompropertycollection/item/
---
## CustomPropertyCollection indexer (1 of 2)

Ottiene la proprietà personalizzata tramite l'indice specifico.

```csharp
public CustomProperty this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

La proprietà personalizzata

### Esempi

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

### Vedi anche

* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## CustomPropertyCollection indexer (2 of 2)

Ottiene la proprietà personalizzata tramite il nome della proprietà.

```csharp
public CustomProperty this[string name] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| name | Il nome della proprietà. |

### Valore di ritorno

La proprietà personalizzata

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi proprietà personalizzate
            worksheet.CustomProperties.Add("COR_Report", "Quarterly Report");
            worksheet.CustomProperties.Add("COR_ResultSet", "Sales Data");
            
            // Accedi e visualizza le proprietà personalizzate usando la proprietà Item
            Console.WriteLine("COR_Report: " + worksheet.CustomProperties["COR_Report"].Value);
            Console.WriteLine("COR_ResultSet: " + worksheet.CustomProperties["COR_ResultSet"].Value);
            
            // Modifica una proprietà personalizzata usando la proprietà Item
            worksheet.CustomProperties["COR_Report"].Value = "Annual Report";
            Console.WriteLine("Updated COR_Report: " + worksheet.CustomProperties["COR_Report"].Value);
        }
    }
}
```

### Vedi anche

* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


