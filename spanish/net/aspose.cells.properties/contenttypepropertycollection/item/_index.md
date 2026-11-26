---
title: "ContentTypePropertyCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ContentTypePropertyCollection. Obtiene la propiedad del tipo de contenido por el índice específico"
type: docs
url: /es/net/aspose.cells.properties/contenttypepropertycollection/item/
---
## ContentTypePropertyCollection indexer (1 of 2)

Obtiene la propiedad del tipo de contenido por el índice específico.

```csharp
public ContentTypeProperty this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

La propiedad del tipo de contenido

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Agregar propiedades del tipo de contenido y demostrar el uso de la propiedad Item
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // Acceder a las propiedades usando el indexador Item
            Console.WriteLine($"Property1 IsNillable: {workbook.ContentTypeProperties[0].IsNillable}");
            Console.WriteLine($"Property2 IsNillable: {workbook.ContentTypeProperties[1].IsNillable}");
            
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## ContentTypePropertyCollection indexer (2 of 2)

Obtiene la propiedad del tipo de contenido por el nombre de la propiedad.

```csharp
public ContentTypeProperty this[string name] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| name | El nombre de la propiedad. |

### Valor de retorno

La propiedad del tipo de contenido

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Agregar propiedad del tipo de contenido
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // Acceder a la propiedad usando el indexador Item
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // Modificar valores de la propiedad
            property.Value = "UpdatedValue";
            property.IsNillable = false;
            
            // Guardar el libro de trabajo
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


