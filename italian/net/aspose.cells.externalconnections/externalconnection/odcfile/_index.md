---
title: "ExternalConnection.OdcFile"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Specifica il percorso completo al file di connessione esterna da cui è stata creata questa connessione. Se una connessione fallisce durante un tentativo di aggiornamento dei dati e reconnectionMethod1, l'applicazione di foglio di calcolo proverà di nuovo utilizzando le informazioni dal file di connessione esterna invece dell'oggetto di connessione incorporato nella cartella di lavoro"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/odcfile/
---
## ExternalConnection.OdcFile property

Specifica il percorso completo al file di connessione esterna da cui è stata creata questa connessione. Se una connessione fallisce durante un tentativo di aggiornamento dei dati, e reconnectionMethod=1, allora l'applicazione di foglio di calcolo proverà di nuovo usando le informazioni dal file di connessione esterna invece dell'oggetto connessione incorporato nel workbook.

```csharp
public string OdcFile { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOdcFileDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione esterna (supponendo che ne esista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visualizza il valore corrente di OdcFile
                Console.WriteLine("Initial OdcFile value: " + connection.OdcFile);
                
                // Imposta un nuovo valore di OdcFile (poiché è leggibile e scrivibile)
                connection.OdcFile = @"C:\Connections\ExternalData.odc";
                Console.WriteLine("Updated OdcFile value: " + connection.OdcFile);
                
                // Cancella il valore di OdcFile
                connection.OdcFile = string.Empty;
                Console.WriteLine("Cleared OdcFile value: " + connection.OdcFile);
                
                // Salva la cartella di lavoro con le impostazioni di connessione modificate
                workbook.Save("OdcFileDemo.xlsx");
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


