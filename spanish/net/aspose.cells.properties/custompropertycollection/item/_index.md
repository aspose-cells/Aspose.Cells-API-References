---
title: "CustomPropertyCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CustomPropertyCollection. Obtiene la propiedad personalizada por el índice específico"
type: docs
url: /es/net/aspose.cells.properties/custompropertycollection/item/
---
## CustomPropertyCollection indexer (1 of 2)

Obtiene la propiedad personalizada por el índice específico.

```csharp
public CustomProperty this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

La propiedad personalizada

### Ejemplos

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

### Ver también

* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## CustomPropertyCollection indexer (2 of 2)

Obtiene la propiedad personalizada por el nombre de la propiedad.

```csharp
public CustomProperty this[string name] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| name | El nombre de la propiedad. |

### Valor de retorno

La propiedad personalizada

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar propiedades personalizadas
            worksheet.CustomProperties.Add("COR_Report", "Quarterly Report");
            worksheet.CustomProperties.Add("COR_ResultSet", "Sales Data");
            
            // Acceder y mostrar propiedades personalizadas usando la propiedad Item
            Console.WriteLine("COR_Report: " + worksheet.CustomProperties["COR_Report"].Value);
            Console.WriteLine("COR_ResultSet: " + worksheet.CustomProperties["COR_ResultSet"].Value);
            
            // Modificar una propiedad personalizada usando la propiedad Item
            worksheet.CustomProperties["COR_Report"].Value = "Annual Report";
            Console.WriteLine("Updated COR_Report: " + worksheet.CustomProperties["COR_Report"].Value);
        }
    }
}
```

### Ver también

* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


