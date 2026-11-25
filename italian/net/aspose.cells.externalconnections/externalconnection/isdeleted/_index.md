---
title: "ExternalConnection.IsDeleted"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Indica se la connessione della cartella di lavoro associata è stata eliminata. true se la connessione è stata eliminata, altrimenti false"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/isdeleted/
---
## ExternalConnection.IsDeleted property

Indica se la connessione del workbook associata è stata eliminata. true se la connessione è stata eliminata; altrimenti, false.

```csharp
public bool IsDeleted { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione esterna (supponendo che ne esista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visualizza il valore iniziale di IsDeleted
                Console.WriteLine("Initial IsDeleted value: " + connection.IsDeleted);
                
                // Attiva/disattiva il valore IsDeleted (poiché è leggibile e scrivibile)
                connection.IsDeleted = !connection.IsDeleted;
                Console.WriteLine("Updated IsDeleted value: " + connection.IsDeleted);
                
                // Salva la cartella di lavoro con le impostazioni di connessione modificate
                workbook.Save("IsDeletedDemo.xlsx");
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


