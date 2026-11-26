---
title: "ConnectionParameterCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConnectionParameterCollection. Obtiene el elemento ConnectionParameter en el índice especificado"
type: docs
url: /es/net/aspose.cells.externalconnections/connectionparametercollection/item/
---
## ConnectionParameterCollection indexer (1 of 2)

Obtiene el elemento [`ConnectionParameter`](../../connectionparameter/) en el índice especificado.

```csharp
public ConnectionParameter this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Obtener la primera conexión externa
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Obtener la colección de parámetros
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Verificar si hay parámetros antes de acceder
                if (parameters.Count > 0)
                {
                    // Demostrar la lectura de la propiedad Item
                    ConnectionParameter firstParam = parameters[0];
                    Console.WriteLine($"Parameter type: {firstParam.GetType().Name}");
                }
                else
                {
                    Console.WriteLine("No parameters in collection");
                }
                
                // Guarda el libro de trabajo
                workbook.Save("ConnectionParameterItemDemo.xlsx");
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

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ConnectionParameterCollection indexer (2 of 2)

Obtiene el elemento [`ConnectionParameter`](../../connectionparameter/) con el nombre especificado.

```csharp
public ConnectionParameter this[string connParamName] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| connParamName | nombre del parámetro de conexión |

### Valor de retorno

El elemento con el nombre especificado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Obtener la primera conexión externa
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Obtener la colección de parámetros
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Verificar si existen parámetros para demostrar la propiedad Item
                if (parameters.Count == 0)
                {
                    Console.WriteLine("No parameters in collection to demonstrate Item property");
                    return;
                }
                
                // Obtener el nombre del primer parámetro para usar en la demostración
                string firstParamName = parameters[0].Name;
                
                // Demostrar la lectura de la propiedad Item por nombre
                ConnectionParameter retrievedParam = parameters[firstParamName];
                
                if (retrievedParam != null)
                {
                    Console.WriteLine($"Retrieved parameter name: {retrievedParam.Name}");
                }
                else
                {
                    Console.WriteLine("Parameter not found");
                }
                
                // Guarda el libro de trabajo
                workbook.Save("ConnectionParameterItemDemo.xlsx");
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

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


