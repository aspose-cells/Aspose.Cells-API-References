---
title: "PivotField.IsAutoShow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Gibt an, ob das angegebene PivotTable-Feld automatisch angezeigt wird"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/isautoshow/
---
## PivotField.IsAutoShow property

Gibt an, ob das angegebene PivotTable-Feld automatisch angezeigt wird.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.IsAutoShow property  or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAutoShow { get; set; }
```

### Hinweise

NOTE: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen bitte die Eigenschaft PivotField.Top10AutoShowSettings.IsAutoShow oder die Methode PivotField.Top10AutoShow(). Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAutoShowDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // PivotTable hinzufügen
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Datenfeld hinzufügen und IsAutoShow konfigurieren
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            
            // AutoShow aktivieren und Einstellungen konfigurieren
            dataField.IsAutoShow = true;
            dataField.AutoShowCount = 2;
            dataField.AutoShowField = 0; // Index of the field to auto show
            dataField.IsAscendShow = true;
            
            // Daten berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Den Wert der IsAutoShow-Eigenschaft ausgeben
            Console.WriteLine("IsAutoShow property value: " + dataField.IsAutoShow);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldPropertyIsAutoShowDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


