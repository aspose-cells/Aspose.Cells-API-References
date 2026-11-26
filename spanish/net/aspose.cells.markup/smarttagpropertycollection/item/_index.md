---
title: "SmartTagPropertyCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SmartTagPropertyCollection. Obtiene un objeto SmartTagProperty"
type: docs
url: /es/net/aspose.cells.markup/smarttagpropertycollection/item/
---
## SmartTagPropertyCollection indexer (1 of 2)

Obtiene un objeto [`SmartTagProperty`](../../smarttagproperty/)

```csharp
public SmartTagProperty this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice |

### Valor de retorno

Devuelve un objeto [`SmartTagProperty`](../../smarttagproperty/).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una colección de propiedades de smart tag
            SmartTagPropertyCollection properties = new SmartTagPropertyCollection();

            // Agrega propiedades a la colección
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // Acceder a las propiedades usando el indexador Item
            SmartTagProperty property1 = properties[index1];
            SmartTagProperty property2 = properties[index2];

            // Mostrar los valores actuales de la propiedad
            Console.WriteLine("Property1 Name: " + property1.Name);
            Console.WriteLine("Property1 Value: " + property1.Value);
            Console.WriteLine("Property2 Name: " + property2.Name);
            Console.WriteLine("Property2 Value: " + property2.Value);

            // Nota: La propiedad Item es de solo lectura, por lo que no podemos asignarle directamente
            // En su lugar, podemos modificar las propiedades de los objetos SmartTagProperty devueltos
            property1.Value = "UpdatedValue1";
            property2.Value = "UpdatedValue2";

            // Mostrar los valores actualizados
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property1 Value: " + properties[index1].Value);
            Console.WriteLine("Property2 Value: " + properties[index2].Value);

            // Guardar el libro de trabajo (aunque los smart tags no se almacenan visiblemente en una guardada simple)
            workbook.Save("SmartTagPropertyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagPropertyCollection indexer (2 of 2)

Obtiene un objeto [`SmartTagProperty`](../../smarttagproperty/) por el nombre de la propiedad.

```csharp
public SmartTagProperty this[string name] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| name | El nombre de la propiedad. |

### Valor de retorno

Devuelve un objeto [`SmartTagProperty`](../../smarttagproperty/).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crear una configuración de smart tag y añadir un smart tag
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
                int smartTagIndex = smartTagSetting.Add(0, 0);
                SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
                smartTags.Add("http://example.com", "example");

                // Obtener el smart tag y sus propiedades
                SmartTag smartTag = smartTags[0];
                SmartTagPropertyCollection properties = smartTag.Properties;

                // Agregar algunas propiedades para demostrar la propiedad Item
                properties.Add("Author", "John Doe");
                properties.Add("Version", "1.0");

                // Acceder a las propiedades usando el indexador Item (por índice)
                SmartTagProperty firstProperty = properties[0];
                SmartTagProperty secondProperty = properties[1];

                // Muestra los valores de la propiedad
                Console.WriteLine("First Property Name: " + firstProperty.Name);
                Console.WriteLine("First Property Value: " + firstProperty.Value);
                Console.WriteLine("Second Property Name: " + secondProperty.Name);
                Console.WriteLine("Second Property Value: " + secondProperty.Value);

                // Guarda el libro de trabajo
                workbook.Save("SmartTagItemDemo.xlsx");
                Console.WriteLine("SmartTagItemDemo.xlsx created successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


