---
title: "DocumentPropertyCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método DocumentPropertyCollection. Elimina una propiedad en el índice especificado"
type: docs
url: /es/net/aspose.cells.properties/documentpropertycollection/removeat/
---
## DocumentPropertyCollection.RemoveAt method

Elimina una propiedad en el índice especificado.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice basado en cero. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a propiedades de documento personalizadas (en lugar de las incorporadas)
            DocumentPropertyCollection properties = workbook.Worksheets.CustomDocumentProperties;
            
            // Agregar algunas propiedades personalizadas para demostrar la eliminación
            ((CustomDocumentPropertyCollection)properties).Add("Property1", "Value1");
            ((CustomDocumentPropertyCollection)properties).Add("Property2", "Value2");
            ((CustomDocumentPropertyCollection)properties).Add("Property3", "Value3");

            try
            {
                // Mostrar propiedades antes de la eliminación
                Console.WriteLine("Properties before removal:");
                foreach (DocumentProperty prop in properties)
                {
                    Console.WriteLine($"{prop.Name}: {prop.Value}");
                }

                // Llamar a RemoveAt con el índice 1 (segunda propiedad)
                properties.RemoveAt(1);

                // Mostrar propiedades después de la eliminación
                Console.WriteLine("\nProperties after removal:");
                foreach (DocumentProperty prop in properties)
                {
                    Console.WriteLine($"{prop.Name}: {prop.Value}");
                }

                Console.WriteLine("RemoveAt method executed successfully with parameter (Int32)");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Error: Index out of range. {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("RemoveAtMethodDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


