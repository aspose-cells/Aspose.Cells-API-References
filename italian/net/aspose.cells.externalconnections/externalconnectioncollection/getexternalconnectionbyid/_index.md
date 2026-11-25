---
title: "ExternalConnectionCollection.GetExternalConnectionById"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ExternalConnectionCollection metodo. Ottiene l'elemento ExternalConnection con l'id specificato"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid/
---
## ExternalConnectionCollection.GetExternalConnectionById method

Ottiene l'elemento [`ExternalConnection`](../../externalconnection/) con l'id specificato.

```csharp
public ExternalConnection GetExternalConnectionById(int connId)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| connId | Int32 | id della connessione esterna |

### Valore di ritorno

L'elemento con l'id specificato.

### Esempi

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
            // Crea un nuovo workbook con connessioni dati di esempio
            Workbook workbook = new Workbook();
            
            // Ottieni la raccolta di connessioni esterne
            ExternalConnectionCollection dataConns = workbook.DataConnections;

            // Crea e aggiungi connessioni utilizzando i metodi API appropriati
            // Nota: In un uso reale, otterresti tipicamente le connessioni esistenti
            // piuttosto che creare nuove in questo modo
            int connectionId1 = 1;
            int connectionId2 = 2;
            
            // Ottieni una connessione specifica per ID (sarà null inizialmente)
            ExternalConnection specificConn = dataConns.GetExternalConnectionById(connectionId1);
            
            if (specificConn == null)
            {
                Console.WriteLine($"No connection found with ID {connectionId1}");
                // In un uso reale, lavoreresti con le connessioni esistenti
                // oppure crearle tramite i metodi API appropriati
            }
            else
            {
                Console.WriteLine($"Found connection: ID={specificConn.ConnectionId}, Name={specificConn.Name}");
                specificConn.Name = "ModifiedConnection";
            }

            // Salva la cartella di lavoro
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


