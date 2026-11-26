---
title: "ContentTypeProperty.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ContentTypeProperty. Devuelve o establece el valor de la propiedad de tipo de contenido"
type: docs
url: /es/net/aspose.cells.properties/contenttypeproperty/value/
---
## ContentTypeProperty.Value property

Devuelve o establece el valor de la propiedad de tipo de contenido.

```csharp
public string Value { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Agregar una propiedad de tipo de contenido
            workbook.ContentTypeProperties.Add("Admin", "InitialValue", "text");
            
            // Acceder y modificar el Valor de la propiedad
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.Value = "Aspose"; // Demonstrating Value property usage
            
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


