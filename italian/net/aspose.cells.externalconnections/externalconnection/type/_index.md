---
title: "ExternalConnection.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Ottiene o imposta il tipo di DataSource della connessione esterna"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/type/
---
## ExternalConnection.Type property

Ottiene o imposta il tipo di DataSource della connessione esterna.

```csharp
[Obsolete("Use ExternalConnection.SourceType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ConnectionDataSourceType Type { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ExternalConnection.SourceType. Questa proprietà sarà rimossa tra 12 mesi a partire da ottobre 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione esterna (supponendo che ne esista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visualizza il valore corrente di Type (operazione di lettura)
                Console.WriteLine("Initial Type value: " + connection.Type);
                
                // Imposta un nuovo valore di Type (poiché è leggibile e scrivibile)
                connection.Type = ConnectionDataSourceType.OLEDBBasedSource;
                Console.WriteLine("Updated Type value: " + connection.Type);
                
                // Scorri i valori possibili per dimostrare la capacità di impostazione
                foreach (ConnectionDataSourceType type in Enum.GetValues(typeof(ConnectionDataSourceType)))
                {
                    if ((int)type != 102) // Skip duplicate enum value
                    {
                        connection.Type = type;
                        Console.WriteLine($"Type set to: {type}");
                    }
                }
                
                // Salva la cartella di lavoro con le impostazioni di connessione modificate
                workbook.Save("TypeDemo.xlsx");
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

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


