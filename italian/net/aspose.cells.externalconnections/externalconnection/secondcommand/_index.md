---
title: "ExternalConnection.SecondCommand"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Specifica una stringa di testo per un secondo comando che viene conservata quando i campi di pagina basati su server di PivotTable sono in uso. Per le connessioni ODBC serverCommand è solitamente una query più ampia rispetto al comando, poiché non è presente alcuna clausola WHERE nella prima. In base a questi 2 comandi, i parametri Command e ServerCommand possono essere usati per popolare l'interfaccia utente e costruire query parametrizzate."
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/secondcommand/
---
## ExternalConnection.SecondCommand property

Specifica una seconda stringa di testo del comando che viene mantenuta quando i campi di pagina basati su server della PivotTable sono in uso. Per le connessioni ODBC, serverCommand è solitamente una query più ampia rispetto a command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed

```csharp
public virtual string SecondCommand { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySecondCommandDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione esterna (supponendo che ne esista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visualizza il valore corrente di SecondCommand (operazione di lettura)
                Console.WriteLine("Initial SecondCommand value: " + connection.SecondCommand);
                
                // Imposta un nuovo valore di SecondCommand (poiché è leggibile e scrivibile)
                connection.SecondCommand = "SELECT * FROM Customers WHERE Country = 'USA'";
                Console.WriteLine("Updated SecondCommand value: " + connection.SecondCommand);
                
                // Cancella SecondCommand per dimostrare l'impostazione di una stringa vuota
                connection.SecondCommand = string.Empty;
                Console.WriteLine("Cleared SecondCommand value: " + connection.SecondCommand);
                
                // Salva la cartella di lavoro con le impostazioni di connessione modificate
                workbook.Save("SecondCommandDemo.xlsx");
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


