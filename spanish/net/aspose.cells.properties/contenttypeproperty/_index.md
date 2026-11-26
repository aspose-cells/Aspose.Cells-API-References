---
title: "Clase ContentTypeProperty"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Properties.ContentTypeProperty class. Representa información de identificador"
type: docs
url: /es/net/aspose.cells.properties/contenttypeproperty/
---
## ContentTypeProperty class

Representa información de identificador.

```csharp
public class ContentTypeProperty
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [IsNillable](../../aspose.cells.properties/contenttypeproperty/isnillable/) { get; set; } | Indica si el valor podría estar vacío. |
| [Name](../../aspose.cells.properties/contenttypeproperty/name/) { get; set; } | Devuelve o establece el nombre del objeto. |
| [Type](../../aspose.cells.properties/contenttypeproperty/type/) { get; set; } | Obtiene y establece el tipo de la propiedad. |
| [Value](../../aspose.cells.properties/contenttypeproperty/value/) { get; set; } | Devuelve o establece el valor de la propiedad de tipo de contenido. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class ContentTypePropertyDemo
    {
        public static void ContentTypePropertyExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Agregar una nueva propiedad de tipo de contenido
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");

            // Acceder a la propiedad recién añadida
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // Estableciendo propiedades
            property.Name = "Admin";
            property.Value = "Aspose";
            property.Type = "text";
            property.IsNillable = true;

            // Guardar el archivo Excel
            workbook.Save("ContentTypePropertyExample.xlsx");
            workbook.Save("ContentTypePropertyExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


