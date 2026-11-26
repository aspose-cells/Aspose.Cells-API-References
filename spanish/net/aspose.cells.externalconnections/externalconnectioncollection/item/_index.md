---
title: "ExternalConnectionCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnectionCollection. Obtiene el elemento ExternalConnection en el índice especificado"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnectioncollection/item/
---
## ExternalConnectionCollection indexer (1 of 2)

Obtiene el elemento [`ExternalConnection`](../../externalconnection/) en el índice especificado.

```csharp
public ExternalConnection this[int index] { get; }
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

    public class ExternalConnectionCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Acceder a la colección de conexiones externas
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Verificar si hay alguna conexión
                if (connections.Count > 0)
                {
                    // Demostrar el acceso a un elemento por índice (operación de lectura)
                    ExternalConnection connection = connections[0];

                    // Muestra la información de la conexión
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                    Console.WriteLine($"Connection ID: {connection.ConnectionId}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }

                // Guarda el libro de trabajo
                workbook.Save("ExternalConnectionItemDemo.xlsx");
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

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ExternalConnectionCollection indexer (2 of 2)

Obtiene el elemento [`ExternalConnection`](../../externalconnection/) con el nombre especificado.

```csharp
public ExternalConnection this[string connectionName] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| connectionName | el nombre de la conexión de datos |

### Valor de retorno

El elemento con el nombre especificado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceder a la colección de conexiones externas
                ExternalConnectionCollection connections = workbook.DataConnections;
                
                // Agregar una conexión de ejemplo (si es necesario para la demostración)
                // Esto asume que la colección permite agregar conexiones
                // connections.Add(new ExternalConnection());
                
                // Demostrar el acceso a un elemento por nombre (operación de lectura)
                // Nota: En un escenario real, necesitarías nombres de conexión reales
                if (connections.Count > 0)
                {
                    // Obtener el primer nombre de conexión (si está disponible)
                    string connectionName = connections[0].Name;
                    
                    // Acceder a la propiedad Item
                    ExternalConnection connection = connections[connectionName];
                    
                    // Muestra la información de la conexión
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }
                
                // Guarda el libro de trabajo
                workbook.Save("ExternalConnectionDemo.xlsx");
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

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


