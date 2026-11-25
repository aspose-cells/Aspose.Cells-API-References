---
title: "ExternalConnection.RefreshInternal"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Specifica il numero di minuti tra gli aggiornamenti automatici della connessione"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/refreshinternal/
---
## ExternalConnection.RefreshInternal property

Specifica il numero di minuti tra gli aggiornamenti automatici della connessione.

```csharp
public int RefreshInternal { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyRefreshInternalDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per rendere l'esempio significativo
            worksheet.Cells["A1"].Value = "Connection Demo";
            
            try
            {
                // Crea una connessione dati (utilizzando la classe base ExternalConnection)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Imposta e visualizza la proprietà RefreshInternal
                connection.RefreshInternal = 30; // Refresh every 30 minutes
                Console.WriteLine("RefreshInternal value: " + connection.RefreshInternal);
                
                // Modifica l'intervallo di aggiornamento
                connection.RefreshInternal = 60;
                Console.WriteLine("Updated RefreshInternal value: " + connection.RefreshInternal);
                
                // Salva la cartella di lavoro con le impostazioni della connessione
                workbook.Save("RefreshInternalDemo.xlsx");
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


