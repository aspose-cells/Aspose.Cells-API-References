---
title: "ContentTypeProperty.IsNillable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ContentTypeProperty. Indica si el valor puede estar vacío"
type: docs
url: /es/net/aspose.cells.properties/contenttypeproperty/isnillable/
---
## ContentTypeProperty.IsNillable property

Indica si el valor podría estar vacío.

```csharp
public bool IsNillable { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyIsNillableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Agregar una propiedad de tipo de contenido
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // Acceder a la propiedad y establecer IsNillable
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.IsNillable = true;
            
            // Verificar y mostrar el valor de IsNillable
            Console.WriteLine($"Property 'Admin' IsNillable: {property.IsNillable}");
            
            workbook.Save("ContentTypePropertyIsNillableDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


