---
title: "WorkbookDesigner.SortDataSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookDesigner‑Eigenschaft. Gibt an, ob die Datenquelle sortiert wird"
type: docs
url: /de/net/aspose.cells/workbookdesigner/sortdatasource/
---
## WorkbookDesigner.SortDataSource property

Gibt an, ob die Datenquelle sortiert wird.

```csharp
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SortDataSource { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Diese Eigenschaft wird 12 Monate später, seit Oktober 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben. JSON‑Datenquelle wird sortiert, wenn der Smart‑Marker aufsteigende und absteigende Parameter enthält.

### Beispiele

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
            // Erstellen Sie eine Beispiel‑DataTable mit unsortierten Daten
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID", typeof(int));
            dataTable.Columns.Add("ProductName", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // Beispieldaten in unsortierter Reihenfolge hinzufügen
            dataTable.Rows.Add(3, "Product C", 15.99m);
            dataTable.Rows.Add(1, "Product A", 10.50m);
            dataTable.Rows.Add(2, "Product B", 12.75m);

            // Eine Arbeitsmappe mit Smart Markern erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Richten Sie Smart‑Marker im Arbeitsblatt ein
            worksheet.Cells["A1"].PutValue("&=$ProductID");
            worksheet.Cells["B1"].PutValue("&=$ProductName");
            worksheet.Cells["C1"].PutValue("&=$Price");

            try
            {
                // WorkbookDesigner-Instanz erstellen
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Anfangswert von SortDataSource anzeigen
                Console.WriteLine($"Initial SortDataSource value: {designer.SortDataSource}");

                // Datenquelle ohne Sortierung festlegen
                designer.SortDataSource = false;
                designer.SetDataSource(dataTable);
                designer.Process();

                // Das unsortierte Ergebnis speichern
                workbook.Save("UnsortedOutput.xlsx");
                Console.WriteLine("Unsorted data saved to UnsortedOutput.xlsx");

                // Eine neue Arbeitsmappe für die sortierte Demonstration erstellen
                Workbook sortedWorkbook = new Workbook();
                Worksheet sortedSheet = sortedWorkbook.Worksheets[0];
                sortedSheet.Cells["A1"].PutValue("&=$ProductID");
                sortedSheet.Cells["B1"].PutValue("&=$ProductName");
                sortedSheet.Cells["C1"].PutValue("&=$Price");

                // Neuen Designer mit aktivierter Sortierung erstellen
                WorkbookDesigner sortedDesigner = new WorkbookDesigner(sortedWorkbook);
                sortedDesigner.SortDataSource = true;
                sortedDesigner.SetDataSource(dataTable);
                sortedDesigner.Process();

                // Das sortierte Ergebnis speichern
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

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


