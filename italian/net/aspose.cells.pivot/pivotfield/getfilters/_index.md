---
title: "PivotField.GetFilters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotField method. Ottiene tutti i filtri pivot applicati a questo campo pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/getfilters/
---
## PivotField.GetFilters method

Recupera tutti i filtri pivot applicati a questo campo pivot.

```csharp
public PivotFilter[] GetFilters()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGetFiltersDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["B1"].Value = "Sales";
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].Value = DateTime.Now.AddDays(i-2);
                worksheet.Cells[$"B{i}"].Value = i * 100;
            }

            // Crea tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B10", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Aggiungi campo riga e campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Applica filtro data
            PivotField dateField = pivotTable.RowFields[0];
            DateTime startDate = DateTime.Now;
            DateTime endDate = DateTime.Now.AddDays(5);
            dateField.FilterByDate(PivotFilterType.DateBetween, startDate, endDate);
            
            // Ottieni e visualizza i filtri
            PivotFilter[] filters = dateField.GetFilters();
            Console.WriteLine($"Number of filters applied: {filters.Length}");
            if (filters.Length > 0)
            {
                Console.WriteLine($"Filter type: {filters[0].FilterType}");
                Console.WriteLine($"Start date: {filters[0].GetDateTimeValues()[0]}");
                Console.WriteLine($"End date: {filters[0].GetDateTimeValues()[1]}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldGetFiltersDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../../pivotfilter/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


