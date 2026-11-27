---
title: "PivotTable.ShowPivotStyleRowStripes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om radrandig formatering tillämpas"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showpivotstylerowstripes/
---
## PivotTable.ShowPivotStyleRowStripes property

Anger om radstripe‑formatering tillämpas.

```csharp
public bool ShowPivotStyleRowStripes { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleRowStripesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata
            DataTable data = new DataTable();
            data.Columns.Add("Category", typeof(string));
            data.Columns.Add("Product", typeof(string));
            data.Columns.Add("Sales", typeof(int));

            data.Rows.Add("Electronics", "Laptop", 1200);
            data.Rows.Add("Electronics", "Phone", 800);
            data.Rows.Add("Clothing", "Shirt", 50);
            data.Rows.Add("Clothing", "Pants", 70);
            data.Rows.Add("Furniture", "Chair", 150);
            data.Rows.Add("Furniture", "Table", 300);

            // Importera data till kalkylbladet
            worksheet.Cells.ImportData(data, 0, 0, new ImportTableOptions());

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:C7", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till rader och kolumner
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Aktivera radrandig formatering
            pivotTable.ShowPivotStyleRowStripes = true;

            // Beräkna data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTableWithRowStripes.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


