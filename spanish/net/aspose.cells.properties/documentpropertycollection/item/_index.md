---
title: "DocumentPropertyCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DocumentPropertyCollection. Devuelve un objeto DocumentProperty por el nombre de la propiedad"
type: docs
url: /es/net/aspose.cells.properties/documentpropertycollection/item/
---
## DocumentPropertyCollection indexer (1 of 2)

Devuelve un objeto [`DocumentProperty`](../../documentproperty/) por el nombre de la propiedad.

```csharp
public virtual DocumentProperty this[string name] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| name | El nombre de la propiedad sin distinción de mayúsculas a recuperar. |

### Observaciones

Devuelve null si no se encuentra una propiedad con el nombre especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            string key = "TemplateGUID";
            object value = "TestValue123";

            if (wb.Worksheets.CustomDocumentProperties.Contains(key))
            {
                wb.Worksheets.CustomDocumentProperties[key].Value = value;
            }
            else
            {
                wb.Worksheets.CustomDocumentProperties.Add(key, value.ToString());
            }

            // Verificar que el valor se haya establecido usando la propiedad Item
            Console.WriteLine("Property Value: " + wb.Worksheets.CustomDocumentProperties[key].Value);
        }
    }
}
```

### Ver también

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## DocumentPropertyCollection indexer (2 of 2)

Devuelve un objeto [`DocumentProperty`](../../documentproperty/) por índice.

```csharp
public DocumentProperty this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| index | Índice basado en cero del [`DocumentProperty`](../../documentproperty/) a recuperar. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Obtener propiedades de documento incorporadas
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Establecer propiedades incorporadas (no Agregar)
            properties.Author = "John Doe";
            properties.Company = "Aspose";
            properties["Version"].Value = "1.0";

            // Acceder a las propiedades usando el indexador Item
            Console.WriteLine("Property 0: " + properties[0].Name + " = " + properties[0].Value);
            Console.WriteLine("Property 1: " + properties[1].Name + " = " + properties[1].Value);
            Console.WriteLine("Property 2: " + properties[2].Name + " = " + properties[2].Value);

            // Accede a la propiedad por nombre
            DocumentProperty authorProp = properties["Author"];
            Console.WriteLine("Author property: " + authorProp.Value);

            // Modificar una propiedad
            properties["Version"].Value = "2.0";
            Console.WriteLine("Updated Version: " + properties["Version"].Value);
        }
    }
}
```

### Ver también

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


