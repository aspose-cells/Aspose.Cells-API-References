---
title: "PivotTable.ShowInOutlineForm"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Formatiert die PivotTable in Gliederungsform."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/showinoutlineform/
---
## PivotTable.ShowInOutlineForm method

Gestaltet die PivotTable in Gliederungsform.

```csharp
public void ShowInOutlineForm()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInOutlineFormDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Beispiel-Datenblatt hinzufügen
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Fügen Sie Beispieldaten hinzu
            dataSheet.Cells["A1"].PutValue("Date");
            dataSheet.Cells["B1"].PutValue("Product");
            dataSheet.Cells["C1"].PutValue("Sales");
            
            dataSheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            dataSheet.Cells["B2"].PutValue("Apple");
            dataSheet.Cells["C2"].PutValue(1000);
            
            dataSheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2));
            dataSheet.Cells["B3"].PutValue("Banana");
            dataSheet.Cells["C3"].PutValue(2000);
            
            dataSheet.Cells["A4"].PutValue(new DateTime(2023, 1, 3));
            dataSheet.Cells["B4"].PutValue("Apple");
            dataSheet.Cells["C4"].PutValue(1500);
            
            // PivotTable-Arbeitsblatt erstellen
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // PivotTable hinzufügen und die Referenz erhalten
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:C4", 
                "A3", 
                "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
                
            // Felder zu Bereichen hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // In Gliederungsform anzeigen
            pivotTable.ShowInOutlineForm();
            
            // Aktualisieren und Daten berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableOutlineFormDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


