---
title: "PivotFilter.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotFilter. Ottiene il nome del filtro pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfilter/name/
---
## PivotFilter.Name property

Ottiene il nome del filtro pivot.

```csharp
public string Name { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyNameDemo
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
            cells["B2"].Value = 100;
            cells["B3"].Value = 200;
            cells["B4"].Value = 300;

            // Aggiungi una tabella pivot
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B4", "D1", "SalesPivot");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aggiungi e configura un filtro pivot
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.Name = "ProductFilter"; // Demonstrating Name property usage
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Aggiorna e calcola i dati pivot
            pivot.RefreshData();
            pivot.CalculateData();

            // Salva la cartella di lavoro
            book.Save("PivotFilterNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


