---
title: "WorkbookDesigner.SortDataSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookDesigner-egenskap. Anger om sortering av datakälla"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/sortdatasource/
---
## WorkbookDesigner.SortDataSource property

Indikerar om datakällan sorteras.

```csharp
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SortDataSource { get; set; }
```

### Anmärkningar

OBS: Den här egenskapen är nu föråldrad. Denna egenskap kommer att tas bort 12 månader senare sedan oktober 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt. Json-datakälla sorteras om smart markör innehåller stigande och fallande parametrar.

### Exempel

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
            // Skapa en exempel-DataTable med osorterade data
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID", typeof(int));
            dataTable.Columns.Add("ProductName", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // Lägg till exempeldata i osorterad ordning
            dataTable.Rows.Add(3, "Product C", 15.99m);
            dataTable.Rows.Add(1, "Product A", 10.50m);
            dataTable.Rows.Add(2, "Product B", 12.75m);

            // Skapa en arbetsbok med smarta markörer
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in smarta markörer i kalkylbladet
            worksheet.Cells["A1"].PutValue("&=$ProductID");
            worksheet.Cells["B1"].PutValue("&=$ProductName");
            worksheet.Cells["C1"].PutValue("&=$Price");

            try
            {
                // Skapa en WorkbookDesigner-instans
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Visa initialt SortDataSource-värde
                Console.WriteLine($"Initial SortDataSource value: {designer.SortDataSource}");

                // Ange datakälla utan sortering
                designer.SortDataSource = false;
                designer.SetDataSource(dataTable);
                designer.Process();

                // Spara det osorterade resultatet
                workbook.Save("UnsortedOutput.xlsx");
                Console.WriteLine("Unsorted data saved to UnsortedOutput.xlsx");

                // Skapa en ny arbetsbok för sorteringsdemonstration
                Workbook sortedWorkbook = new Workbook();
                Worksheet sortedSheet = sortedWorkbook.Worksheets[0];
                sortedSheet.Cells["A1"].PutValue("&=$ProductID");
                sortedSheet.Cells["B1"].PutValue("&=$ProductName");
                sortedSheet.Cells["C1"].PutValue("&=$Price");

                // Skapa en ny designer med sortering aktiverad
                WorkbookDesigner sortedDesigner = new WorkbookDesigner(sortedWorkbook);
                sortedDesigner.SortDataSource = true;
                sortedDesigner.SetDataSource(dataTable);
                sortedDesigner.Process();

                // Spara det sorterade resultatet
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

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


