---
title: "ExternalConnection.Credentials"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Specifica il metodo di autenticazione da utilizzare quando si stabilisce o si ristabilisce la connessione"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/credentials/
---
## ExternalConnection.Credentials property

Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o si ristabilisce) la connessione.

```csharp
[Obsolete("Use ExternalConnection.CredentialsMethodType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CredentialsMethodType Credentials { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ExternalConnection.CredentialsMethodType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da ottobre 2017. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyCredentialsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione esterna (supponendo che ne esista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visualizza il valore corrente di Credentials
                Console.WriteLine("Initial Credentials value: " + connection.Credentials);
                
                // Imposta un nuovo valore di Credentials (poiché è leggibile e scrivibile)
                connection.Credentials = CredentialsMethodType.Integrated;
                Console.WriteLine("Updated Credentials value: " + connection.Credentials);
                
                // Scorri i valori possibili
                foreach (CredentialsMethodType method in Enum.GetValues(typeof(CredentialsMethodType)))
                {
                    connection.Credentials = method;
                    Console.WriteLine($"Credentials set to: {method}");
                }
                
                // Salva la cartella di lavoro con le impostazioni di connessione modificate
                workbook.Save("CredentialsDemo.xlsx");
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

* enum [CredentialsMethodType](../../credentialsmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


