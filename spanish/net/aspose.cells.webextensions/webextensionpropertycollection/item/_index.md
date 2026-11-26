---
title: "WebExtensionPropertyCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionPropertyCollection. Obtiene la propiedad de la extensión web por el índice"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionpropertycollection/item/
---
## WebExtensionPropertyCollection indexer (1 of 2)

Obtiene la propiedad de la extensión web por el índice.

```csharp
public WebExtensionProperty this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

La propiedad de la extensión web.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una colección de propiedades de extensión web
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Agregar algunas propiedades
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // Acceder a las propiedades usando el indexador Item
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // Modificar los valores de las propiedades a través de la colección
            properties[index1].Value = "UpdatedValue1";
            properties[index2].Value = "UpdatedValue2";

            // Demostrar los cambios
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // Guardar el libro de trabajo (aunque las propiedades de la extensión web no serán visibles en el archivo guardado sin una configuración adecuada)
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)

---

## WebExtensionPropertyCollection indexer (2 of 2)

Obtiene la propiedad de la extensión web.

```csharp
public WebExtensionProperty this[string name] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| name | El nombre de la propiedad. |

### Valor de retorno

La propiedad de la extensión web.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una colección de propiedades de extensión web
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Agrega propiedades a la colección
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");

            // Acceder a las propiedades usando el indexador Item
            WebExtensionProperty property1 = properties["Property1"];
            Console.WriteLine("Property1 value: " + property1.Value);

            WebExtensionProperty property2 = properties["Property2"];
            Console.WriteLine("Property2 value: " + property2.Value);

            // Modificar los valores de las propiedades (nota: Item es de solo lectura, por lo que necesitamos usar Agregar/Eliminar)
            properties.RemoveAt("Property1");
            properties.Add("Property1", "NewValue1");

            // Mostrar el valor actualizado
            property1 = properties["Property1"];
            Console.WriteLine("Updated Property1 value: " + property1.Value);

            // Guarda el libro de trabajo
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


