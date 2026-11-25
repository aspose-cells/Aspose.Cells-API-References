---
title: "ExternalConnectionCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnectionCollection. Ottiene l'elemento ExternalConnection all'indice specificato"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnectioncollection/item/
---
## ExternalConnectionCollection indexer (1 of 2)

Ottiene l'elemento [`ExternalConnection`](../../externalconnection/) all'indice specificato.

```csharp
public ExternalConnection this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            try
            {
                // Accedi alla raccolta di connessioni esterne
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Verifica se ci sono connessioni
                if (connections.Count > 0)
                {
                    // Dimostra l'accesso a un elemento per indice (operazione di lettura)
                    ExternalConnection connection = connections[0];

                    // Visualizza le informazioni sulla connessione
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                    Console.WriteLine($"Connection ID: {connection.ConnectionId}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }

                // Salva la cartella di lavoro
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

### Vedi anche

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ExternalConnectionCollection indexer (2 of 2)

Ottiene l'elemento [`ExternalConnection`](../../externalconnection/) con il nome specificato.

```csharp
public ExternalConnection this[string connectionName] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| connectionName | il nome della connessione dati |

### Valore di ritorno

L'elemento con il nome specificato.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla raccolta di connessioni esterne
                ExternalConnectionCollection connections = workbook.DataConnections;
                
                // Aggiungi una connessione di esempio (se necessario per la dimostrazione)
                // Questo presuppone che la raccolta consenta l'aggiunta di connessioni
                // connections.Add(new ExternalConnection());
                
                // Dimostra l'accesso a un elemento per nome (operazione di lettura)
                // Nota: In uno scenario reale, avresti bisogno di nomi di connessione effettivi
                if (connections.Count > 0)
                {
                    // Ottieni il primo nome di connessione (se disponibile)
                    string connectionName = connections[0].Name;
                    
                    // Accedi alla proprietà Item
                    ExternalConnection connection = connections[connectionName];
                    
                    // Visualizza le informazioni sulla connessione
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }
                
                // Salva la cartella di lavoro
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

### Vedi anche

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


