---
title: "PivotTable.FieldListSortAscending"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob Felder in der PivotTable in einer nicht‑Standardreihenfolge in der Feldliste sortiert sind."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/fieldlistsortascending/
---
## PivotTable.FieldListSortAscending property

Gibt an, ob Felder in der PivotTable in der Feldliste in einer nicht‑Standardreihenfolge sortiert sind.

```csharp
public bool FieldListSortAscending { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyFieldListSortAscendingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["B2"].Value = "Laptop";
            worksheet.Cells["C2"].Value = 1200;
            
            worksheet.Cells["A3"].Value = "Electronics";
            worksheet.Cells["B3"].Value = "Phone";
            worksheet.Cells["C3"].Value = 800;
            
            worksheet.Cells["A4"].Value = "Furniture";
            worksheet.Cells["B4"].Value = "Chair";
            worksheet.Cells["C4"].Value = 150;
            
            worksheet.Cells["A5"].Value = "Furniture";
            worksheet.Cells["B5"].Value = "Table";
            worksheet.Cells["C5"].Value = 250;

            // Erstelle eine Pivot-Tabelle
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aktuellen Wert von FieldListSortAscending anzeigen
            Console.WriteLine("Initial FieldListSortAscending: " + pivotTable.FieldListSortAscending);

            // Feldliste in aufsteigender Reihenfolge anzeigen
            pivotTable.FieldListSortAscending = true;
            Console.WriteLine("FieldListSortAscending set to: " + pivotTable.FieldListSortAscending);

            // Aktualisiere und berechne die Pivot-Tabelle
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableFieldListSortAscendingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


