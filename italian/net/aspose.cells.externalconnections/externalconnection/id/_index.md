---
title: "ExternalConnection.Id"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Ottiene l'ID della connessione"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/id/
---
## ExternalConnection.Id property

Ottiene l'ID della connessione.

```csharp
public int Id { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            try
            {
                // Accedi alla prima connessione esterna (la cartella di lavoro include connessioni predefinite)
                ExternalConnection connection = workbook.DataConnections[0];

                // Visualizza il valore corrente di Id (proprietà di sola lettura)
                Console.WriteLine("External Connection Id: " + connection.Id);

                // Visualizza altre proprietà di sola lettura per contesto
                Console.WriteLine("Connection Class Type: " + connection.ClassType);
                Console.WriteLine("Connection Name: " + connection.Name);

                // Salva la cartella di lavoro
                workbook.Save("ExternalConnectionIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with connection Id: " + connection.Id);
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


