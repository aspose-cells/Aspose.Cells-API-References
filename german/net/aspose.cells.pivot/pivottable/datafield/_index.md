---
title: "PivotTable.DataField"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable‑Eigenschaft. Gibt ein PivotField‑Objekt zurück, das alle Datenfelder in einer PivotTable darstellt. Nur lesbar. Es wird nur erstellt, wenn im Datenbereich zwei oder mehr Datenfelder vorhanden sind. Standardmäßig befindet es sich im Zeilenbereich. Sie können es mit der Methode PivotTable.AddFieldToArea in den Zeilen‑/Spaltenbereich ziehen."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/datafield/
---
## PivotTable.DataField property

Gibt ein [`PivotField`](../../pivotfield/)‑Objekt zurück, das alle Datenfelder in einer PivotTable darstellt. Nur lesbar. Es wird nur erstellt, wenn im Datenbereich zwei oder mehr Datenfelder vorhanden sind. Standardmäßig befindet es sich im Zeilenbereich. Sie können es mit der Methode PivotTable.AddFieldToArea() in den Zeilen‑/Spaltenbereich ziehen.

```csharp
[Obsolete("Use PivotTable.ValuesField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotField DataField { get; }
```

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die PivotTable.ValuesField‑Eigenschaft. Diese Methode wird 12 Monate später, seit Oktober 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataFieldDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
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
            
            // Zugriff auf und Änderung von DataField‑Eigenschaften
            // Position ist schreibgeschützt, daher zeigen wir andere Eigenschaften
            pivotTable.DataField.DisplayName = "Total Sales";
            pivotTable.DataField.NumberFormat = "#,##0";
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableDataFieldDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


