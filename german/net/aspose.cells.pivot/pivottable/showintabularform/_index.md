---
title: "PivotTable.ShowInTabularForm"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Ordnet die PivotTable in tabellarischer Form an"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/showintabularform/
---
## PivotTable.ShowInTabularForm method

Gestaltet die PivotTable in Tabellenform.

```csharp
public void ShowInTabularForm()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInTabularFormDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Daten-Arbeitsblatt hinzufügen
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            dataSheet.Cells["A1"].PutValue("Label");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);

            // Pivot-Tabellenblatt hinzufügen
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // PivotTable hinzufügen
            int pivotIndex = pivotSheet.PivotTables.Add("=Data!A1:B3", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Felder zur Pivot-Tabelle hinzufügen
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Label");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // PivotTable in tabellarischer Form anzeigen
            pivotTable.ShowInTabularForm();
            
            // Pivot-Tabellendaten aktualisieren und berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableShowInTabularFormDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


