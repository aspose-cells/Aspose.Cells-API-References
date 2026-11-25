---
title: "WorkbookDesigner.SortDataSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà di WorkbookDesigner. Indica se l'origine dati è ordinata"
type: docs
url: /it/net/aspose.cells/workbookdesigner/sortdatasource/
---
## WorkbookDesigner.SortDataSource property

Indica se l'origine dati è ordinata.

```csharp
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SortDataSource { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Questa proprietà sarà rimossa 12 mesi dopo, a partire da ottobre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato. L'origine dati Json verrà ordinata se il marker intelligente contiene parametri ascendente e discendente.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class WorkbookDesignerPropertySortDataSourceDemo
    {
        public static void Run()
        {
            // Crea una DataTable di esempio con dati non ordinati
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID", typeof(int));
            dataTable.Columns.Add("ProductName", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // Aggiungi dati di esempio in ordine non ordinato
            dataTable.Rows.Add(3, "Product C", 15.99m);
            dataTable.Rows.Add(1, "Product A", 10.50m);
            dataTable.Rows.Add(2, "Product B", 12.75m);

            // Crea un workbook con marker intelligenti
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Configura gli smart marker nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("&=$ProductID");
            worksheet.Cells["B1"].PutValue("&=$ProductName");
            worksheet.Cells["C1"].PutValue("&=$Price");

            try
            {
                // Crea un'istanza di WorkbookDesigner
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Visualizza il valore iniziale di SortDataSource
                Console.WriteLine($"Initial SortDataSource value: {designer.SortDataSource}");

                // Imposta l'origine dati senza ordinamento
                designer.SortDataSource = false;
                designer.SetDataSource(dataTable);
                designer.Process();

                // Salva il risultato non ordinato
                workbook.Save("UnsortedOutput.xlsx");
                Console.WriteLine("Unsorted data saved to UnsortedOutput.xlsx");

                // Crea un nuovo workbook per la dimostrazione ordinata
                Workbook sortedWorkbook = new Workbook();
                Worksheet sortedSheet = sortedWorkbook.Worksheets[0];
                sortedSheet.Cells["A1"].PutValue("&=$ProductID");
                sortedSheet.Cells["B1"].PutValue("&=$ProductName");
                sortedSheet.Cells["C1"].PutValue("&=$Price");

                // Crea un nuovo designer con ordinamento abilitato
                WorkbookDesigner sortedDesigner = new WorkbookDesigner(sortedWorkbook);
                sortedDesigner.SortDataSource = true;
                sortedDesigner.SetDataSource(dataTable);
                sortedDesigner.Process();

                // Salva il risultato ordinato
                sortedWorkbook.Save("SortedOutput.xlsx");
                Console.WriteLine("Sorted data saved to SortedOutput.xlsx");
                Console.WriteLine($"Final SortDataSource value: {sortedDesigner.SortDataSource}");
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

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


