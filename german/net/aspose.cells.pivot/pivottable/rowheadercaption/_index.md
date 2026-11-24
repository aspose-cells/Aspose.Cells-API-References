---
title: "PivotTable.RowHeaderCaption"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt die benutzerdefinierte Beschriftung des Zeilenkopfes in dieser PivotTable zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/rowheadercaption/
---
## PivotTable.RowHeaderCaption property

Liest und schreibt die benutzerdefinierte Beschriftung des Zeilenkopfes in dieser PivotTable.

```csharp
public string RowHeaderCaption { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowHeaderCaptionDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Daten-Arbeitsblatt hinzufügen
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Fügen Sie Beispieldaten hinzu
            var cells = dataSheet.Cells;
            cells["A1"].PutValue("State");
            cells["B1"].PutValue("City");
            cells["C1"].PutValue("Population");
            
            cells["A2"].PutValue("TN");
            cells["B2"].PutValue("Chennai");
            cells["C2"].PutValue("50");
            
            cells["A3"].PutValue("KL");
            cells["B3"].PutValue("Cochin");
            cells["C3"].PutValue("70");
            
            // PivotTable-Arbeitsblatt hinzufügen
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Pivot-Tabelle hinzufügen und ihren Index abrufen
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:C3", 
                "A3", 
                "PivotTable");
            
            // PivotTable-Instanz abrufen
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // PivotTable konfigurieren
            pivotTable.RowHeaderCaption = "State"; // Demonstrating RowHeaderCaption property
            pivotTable.AddFieldToArea(PivotFieldType.Row, "State");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Population");
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableWithRowHeaderCaption.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


