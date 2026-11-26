---
title: "ContentTypeProperty.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ContentTypeProperty. Obtiene y establece el tipo de la propiedad"
type: docs
url: /es/net/aspose.cells.properties/contenttypeproperty/type/
---
## ContentTypeProperty.Type property

Obtiene y establece el tipo de la propiedad.

```csharp
public string Type { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Agregar propiedades de tipo de contenido con diferentes tipos
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            workbook.ContentTypeProperties.Add("Version", "1.0", "number");
            workbook.ContentTypeProperties.Add("Enabled", "true", "boolean");

            // Acceder y mostrar los tipos de propiedad
            foreach (ContentTypeProperty property in workbook.ContentTypeProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

            // Guarda el libro de trabajo
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


