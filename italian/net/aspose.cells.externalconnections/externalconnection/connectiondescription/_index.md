---
title: "ExternalConnection.ConnectionDescription"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Specifica la descrizione fornita dall'utente per questa connessione"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/connectiondescription/
---
## ExternalConnection.ConnectionDescription property

Specifica la descrizione utente per questa connessione

```csharp
public string ConnectionDescription { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.Pivot;
    using System;

    public class ExternalConnectionPropertyConnectionDescriptionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            try
            {
                // Aggiungi un foglio di lavoro con dati di esempio
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["B1"].Value = "Sales";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["B2"].Value = 1000;
                worksheet.Cells["A3"].Value = "Banana";
                worksheet.Cells["B3"].Value = 2000;

                // Crea una tabella pivot per stabilire una connessione esterna
                int pivotIndex = worksheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
                Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Ottieni la connessione esterna dalla tabella pivot
                ExternalConnection connection = pivotTable.GetSourceDataConnections()[0];

                // Visualizza il valore iniziale di ConnectionDescription
                Console.WriteLine("Initial ConnectionDescription: " + connection.ConnectionDescription);

                // Imposta una nuova descrizione (poiché è leggibile e scrivibile)
                connection.ConnectionDescription = "This connection retrieves sales data from internal sources";
                Console.WriteLine("Updated ConnectionDescription: " + connection.ConnectionDescription);

                // Cancella la descrizione
                connection.ConnectionDescription = string.Empty;
                Console.WriteLine("Cleared ConnectionDescription: " + connection.ConnectionDescription);

                // Salva la cartella di lavoro con la connessione modificata
                workbook.Save("ConnectionDescriptionDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


