---
title: "PivotFilter.UseWholeDay"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotFilter property. Indica se utilizzare giorni interi nei criteri di filtraggio della data"
type: docs
url: /it/net/aspose.cells.pivot/pivotfilter/usewholeday/
---
## PivotFilter.UseWholeDay property

Indica se utilizzare giorni interi nei criteri di filtraggio della data.

```csharp
public bool UseWholeDay { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyUseWholeDayDemo
    {
        public static void Run()
        {
            // Crea cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Crea dati di esempio
            cells["A1"].Value = "Date";
            cells["B1"].Value = "Amount";
            cells["A2"].Value = new DateTime(2023, 1, 15);
            cells["A3"].Value = new DateTime(2023, 1, 20);
            cells["A4"].Value = new DateTime(2023, 2, 5);
            cells["A5"].Value = new DateTime(2023, 2, 10);
            cells["B2"].Value = 100;
            cells["B3"].Value = 200;
            cells["B4"].Value = 300;
            cells["B5"].Value = 400;

            // Crea tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "H3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount field
            
            // Aggiungi filtro pivot
            int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.DateBetween);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            filter.Value1 = "2023-01-01";
            filter.Value2 = "2023-01-31";
            
            // Imposta e dimostra la proprietà UseWholeDay
            filter.UseWholeDay = true;
            Console.WriteLine($"UseWholeDay value after setting: {filter.UseWholeDay}");

            // Salva cartella di lavoro
            workbook.Save("PivotFilterUseWholeDayDemo.xlsx");
            
            // Ricarica per verificare la persistenza
            Workbook verifyWorkbook = new Workbook("PivotFilterUseWholeDayDemo.xlsx");
            PivotTable verifyPivot = verifyWorkbook.Worksheets[0].PivotTables[0];
            PivotFilter verifyFilter = verifyPivot.PivotFilters[0];
            Console.WriteLine($"UseWholeDay value after reloading: {verifyFilter.UseWholeDay}");
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


