---
title: "ExternalConnectionCollection.GetExternalConnectionById"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ExternalConnectionCollection. Obtiene el elemento ExternalConnection con el id especificado"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid/
---
## ExternalConnectionCollection.GetExternalConnectionById method

Obtiene el elemento [`ExternalConnection`](../../externalconnection/) con el id especificado.

```csharp
public ExternalConnection GetExternalConnectionById(int connId)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| connId | Int32 | id de conexión externa |

### Valor de retorno

El elemento con el id especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionCollectionMethodGetExternalConnectionByIdWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con conexiones de datos de ejemplo
            Workbook workbook = new Workbook();
            
            // Obtener la colección de conexiones externas
            ExternalConnectionCollection dataConns = workbook.DataConnections;

            // Crear y agregar conexiones usando los métodos de API adecuados
            // Nota: En uso real, normalmente obtendrías conexiones existentes
            // en lugar de crear nuevas de esta manera
            int connectionId1 = 1;
            int connectionId2 = 2;
            
            // Obtener una conexión específica por ID (será nulo inicialmente)
            ExternalConnection specificConn = dataConns.GetExternalConnectionById(connectionId1);
            
            if (specificConn == null)
            {
                Console.WriteLine($"No connection found with ID {connectionId1}");
                // En uso real, trabajarías con conexiones existentes
                // o crearlas mediante los métodos de API adecuados
            }
            else
            {
                Console.WriteLine($"Found connection: ID={specificConn.ConnectionId}, Name={specificConn.Name}");
                specificConn.Name = "ModifiedConnection";
            }

            // Guarda el libro de trabajo
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


