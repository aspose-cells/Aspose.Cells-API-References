---
title: "ExternalConnection.SaveData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. True se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati con la cartella di lavoro, altrimenti false"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/savedata/
---
## ExternalConnection.SaveData property

True se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati con la cartella di lavoro; altrimenti, false.

```csharp
public bool SaveData { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySaveDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione esterna (supponendo che ne esista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visualizza il valore corrente di SaveData
                Console.WriteLine("Initial SaveData value: " + connection.SaveData);
                
                // Dimostra l'impostazione della proprietà (poiché è leggibile e scrivibile)
                connection.SaveData = !connection.SaveData;
                Console.WriteLine("Updated SaveData value: " + connection.SaveData);
                
                // Salva la cartella di lavoro con le impostazioni di connessione modificate
                workbook.Save("SaveDataDemo.xlsx");
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


