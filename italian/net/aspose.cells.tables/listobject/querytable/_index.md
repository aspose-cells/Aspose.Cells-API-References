---
title: "ListObject.QueryTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Ottiene la QueryTable collegata"
type: docs
url: /it/net/aspose.cells.tables/listobject/querytable/
---
## ListObject.QueryTable property

Ottiene la QueryTable collegata.

```csharp
public QueryTable QueryTable { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectPropertyQueryTableDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea un oggetto elenco
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            try
            {
                // Accedi alla proprietà QueryTable (sola lettura)
                QueryTable queryTable = listObject.QueryTable;

                if (queryTable != null)
                {
                    // Visualizza le proprietà della QueryTable
                    Console.WriteLine("QueryTable Name: " + queryTable.Name);
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                    Console.WriteLine("Preserve Formatting: " + queryTable.PreserveFormatting);
                    Console.WriteLine("Adjust Column Width: " + queryTable.AdjustColumnWidth);

                    // Accedi all'intervallo di risultato se disponibile
                    if (queryTable.ResultRange != null)
                    {
                        Console.WriteLine("Result Range Address: " + queryTable.ResultRange.Name);
                    }
                }
                else
                {
                    Console.WriteLine("No QueryTable associated with this ListObject");
                }

                // Salva la cartella di lavoro
                workbook.Save("QueryTableDemo.xlsx");
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

* class [QueryTable](../../../aspose.cells/querytable/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


