---
title: "DocumentPropertyCollection.IndexOf"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método DocumentPropertyCollection. Obtiene el índice de una propiedad por nombre"
type: docs
url: /es/net/aspose.cells.properties/documentpropertycollection/indexof/
---
## DocumentPropertyCollection.IndexOf method

Obtiene el índice de una propiedad por nombre.

```csharp
public int IndexOf(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la propiedad sin distinción de mayúsculas. |

### Valor de retorno

El índice basado en cero. Valor negativo si no se encuentra.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyCollectionMethodIndexOfWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Obtener la colección de propiedades de documento incorporadas
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;

            // Para propiedades incorporadas, solo podemos establecer valores de propiedades existentes
            // Para agregar propiedades personalizadas, necesitaríamos usar CustomDocumentPropertyCollection
            // Aquí solo estableceremos algunas propiedades incorporadas existentes para demostración
            properties["Title"].Value = "Value1";
            properties["Subject"].Value = "Value2";
            properties["Author"].Value = "Value3";

            try
            {
                // Llamar al método IndexOf con un parámetro de cadena
                int index = properties.IndexOf("Subject");
                
                // Mostrar el resultado
                Console.WriteLine($"Index of 'Subject': {index}");
                
                // Mostrar la propiedad en el índice encontrado
                if (index >= 0)
                {
                    DocumentProperty property = properties[index];
                    Console.WriteLine($"Property at index {index}: {property.Name} = {property.Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IndexOf method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("DocumentPropertyIndexOfDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


