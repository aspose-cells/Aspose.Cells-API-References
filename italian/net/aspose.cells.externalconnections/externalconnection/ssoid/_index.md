---
title: "ExternalConnection.SSOId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Identificatore per Single Sign On (SSO) utilizzato per l'autenticazione tra un server spreadsheetML intermedio e la fonte dati esterna"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/ssoid/
---
## ExternalConnection.SSOId property

Identificatore per Single Sign On (SSO) utilizzato per l'autenticazione tra un server spreadsheetML intermedio e la fonte di dati esterna.

```csharp
public string SSOId { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySSOIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione esterna
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visualizza il valore iniziale di SSOId (probabilmente null per una nuova connessione)
                Console.WriteLine("Initial SSOId value: " + connection.SSOId);
                
                // Imposta un nuovo valore SSOId (poiché è leggibile e scrivibile)
                connection.SSOId = "sso-12345";
                Console.WriteLine("Updated SSOId value: " + connection.SSOId);
                
                // Cancella il SSOId
                connection.SSOId = null;
                Console.WriteLine("Cleared SSOId value: " + connection.SSOId);
                
                // Salva la cartella di lavoro con le impostazioni di connessione modificate
                workbook.Save("SSOIdDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


