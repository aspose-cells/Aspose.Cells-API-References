---
title: "PivotTable.ShowEmptyRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob leere Zeilen in die Tabelle aufgenommen werden"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/showemptyrow/
---
## PivotTable.ShowEmptyRow property

Gibt an, ob leere Zeilen in die Tabelle aufgenommen werden sollen.

```csharp
public bool ShowEmptyRow { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowEmptyRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten mit einigen leeren Zeilen hinzufügen
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["B2"].Value = "TV";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Electronics";
            worksheet.Cells["B3"].Value = "";
            worksheet.Cells["C3"].Value = "";
            
            worksheet.Cells["A4"].Value = "Furniture";
            worksheet.Cells["B4"].Value = "Chair";
            worksheet.Cells["C4"].Value = 500;
            
            worksheet.Cells["A5"].Value = "Furniture";
            worksheet.Cells["B5"].Value = "";
            worksheet.Cells["C5"].Value = "";

            // Erstelle eine Pivot-Tabelle
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aktuellen ShowEmptyRow-Wert anzeigen
            Console.WriteLine("Initial ShowEmptyRow value: " + pivotTable.ShowEmptyRow);

            // Leere Zeilen in der PivotTable anzeigen
            pivotTable.ShowEmptyRow = true;
            Console.WriteLine("ShowEmptyRow set to: " + pivotTable.ShowEmptyRow);

            // Daten berechnen, um die Pivot-Tabelle zu füllen
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableShowEmptyRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


