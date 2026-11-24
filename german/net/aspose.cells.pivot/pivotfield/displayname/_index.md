---
title: "PivotField.DisplayName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Stellt den Anzeigenamen des Pivot-Feldes in der PivotTable-Ansicht dar"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/displayname/
---
## PivotField.DisplayName property

Stellt den Anzeigenamen des Pivot-Felds in der PivotTable-Ansicht dar.

```csharp
public string DisplayName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDisplayNameDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe und füge Beispieldaten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // Pivot-Tabelle erstellen
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Zeilenfeld und Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Benutzerdefinierten Anzeigenamen für das Datenfeld festlegen
            pivotTable.DataFields[0].DisplayName = "Total Sales";
            
            // Pivot-Tabelle aktualisieren und berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Zelle über den Anzeigenamen zugreifen
            Cell cell = pivotTable.GetCellByDisplayName("Total Sales");
            Console.WriteLine("Cell found at row: {0}, column: {1}", cell.Row, cell.Column);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldDisplayNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


