---
title: "WebExtensionPropertyCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WebExtensionPropertyCollection. Elimina la propiedad por su nombre"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionpropertycollection/removeat/
---
## WebExtensionPropertyCollection.RemoveAt method

Elimina la propiedad por nombre.

```csharp
public void RemoveAt(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la propiedad. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una colección de propiedades de extensión web
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Añadir algunas propiedades a la colección
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");
            properties.Add("Property3", "Value3");

            try
            {
                // Llamar al método RemoveAt con un parámetro string
                properties.RemoveAt("Property2");

                Console.WriteLine("Property with name 'Property2' removed successfully.");
                
                // Mostrar las propiedades restantes
                Console.WriteLine("Remaining properties:");
                for (int i = 0; i < properties.Count; i++)
                {
                    Console.WriteLine($"{properties[i].Name}: {properties[i].Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("WebExtensionPropertyCollectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


