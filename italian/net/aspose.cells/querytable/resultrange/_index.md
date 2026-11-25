---
title: "QueryTable.ResultRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà QueryTable. Ottiene l'intervallo del risultato"
type: docs
url: /it/net/aspose.cells/querytable/resultrange/
---
## QueryTable.ResultRange property

Ottiene l'intervallo del risultato.

```csharp
public Range ResultRange { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyResultRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per simulare una tabella di query
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            try
            {
                // Verifica se ci sono tabelle query nel foglio di lavoro
                if (worksheet.QueryTables.Count > 0)
                {
                    // Ottieni la prima tabella query
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Mostra il valore della proprietà ResultRange (operazione di sola lettura)
                    Aspose.Cells.Range resultRange = queryTable.ResultRange;
                    Console.WriteLine("ResultRange Address: " + resultRange.Address);
                    Console.WriteLine("ResultRange Row Count: " + resultRange.RowCount);
                    Console.WriteLine("ResultRange Column Count: " + resultRange.ColumnCount);
                    Console.WriteLine("ResultRange First Row: " + resultRange.FirstRow);
                    Console.WriteLine("ResultRange First Column: " + resultRange.FirstColumn);

                    // Visualizza i valori nell'intervallo di risultato
                    Console.WriteLine("Values in ResultRange:");
                    foreach (Cell cell in resultRange)
                    {
                        Console.WriteLine($"Cell [{cell.Row}, {cell.Column}]: {cell.Value}");
                    }
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Salva la cartella di lavoro
                workbook.Save("ResultRangeDemo.xlsx");
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

* class [Range](../../range/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


