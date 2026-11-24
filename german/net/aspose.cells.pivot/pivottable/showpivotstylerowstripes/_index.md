---
title: "PivotTable.ShowPivotStyleRowStripes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob Zeilenstreifenformatierung angewendet wird"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/showpivotstylerowstripes/
---
## PivotTable.ShowPivotStyleRowStripes property

Gibt an, ob Zeilenstreifenformatierung angewendet wird.

```csharp
public bool ShowPivotStyleRowStripes { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle Beispieldaten
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

            // Daten in Arbeitsblatt importieren
            worksheet.Cells.ImportData(data, 0, 0, new ImportTableOptions());

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:C7", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Zeilen und Spalten hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Zeilenstreifen aktivieren
            pivotTable.ShowPivotStyleRowStripes = true;

            // Daten berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableWithRowStripes.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


