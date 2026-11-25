---
title: "PivotFilter.Value1"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotFilter. Ottiene il valore stringa value1 del filtro pivot dell'etichetta"
type: docs
url: /it/net/aspose.cells.pivot/pivotfilter/value1/
---
## PivotFilter.Value1 property

Ottiene il valore stringa1 dell'etichetta del filtro pivot.

```csharp
public string Value1 { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyValue1Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Popola il foglio di lavoro con dati di esempio
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Banana";
            cells["A4"].Value = "Orange";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;

            // Aggiungi una tabella pivot
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B4", "D1", "SalesPivot");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aggiungi un filtro pivot e imposta Value1
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.Value1 = "Apple"; // Filter for Apple products only

            // Aggiorna e calcola i dati
            pivot.RefreshData();
            pivot.CalculateData();

            // Salva la cartella di lavoro
            book.Save("PivotFilterValue1Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


