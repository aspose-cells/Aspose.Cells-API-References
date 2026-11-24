---
title: "PivotTable.SubtotalHiddenPageItems"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob ausgeblendete Seitenfeld-Elemente im PivotTable-Bericht in Zeilen- und Spalten-Teilsummen, Blocksummen und Gesamtsummen einbezogen werden. Der Standardwert ist False."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/subtotalhiddenpageitems/
---
## PivotTable.SubtotalHiddenPageItems property

Gibt an, ob ausgeblendete Seitenfeld-Elemente im PivotTable-Bericht in Zeilen- und Spalten-Teilsummen, Blocksummen und Gesamtsummen einbezogen werden. Der Standardwert ist False.

```csharp
public bool SubtotalHiddenPageItems { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertySubtotalHiddenPageItemsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Apple";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Orange";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            
            cells["A4"].Value = "Banana";
            cells["B4"].Value = "North";
            cells["C4"].Value = 1500;
            
            cells["A5"].Value = "Apple";
            cells["B5"].Value = "South";
            cells["C5"].Value = 1200;

            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Felder hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // SubtotalHiddenPageItems-Eigenschaft festlegen
            pivotTable.SubtotalHiddenPageItems = true;
            Console.WriteLine("SubtotalHiddenPageItems set to: " + pivotTable.SubtotalHiddenPageItems);

            // Aktualisieren und Daten berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTable_SubtotalHiddenPageItemsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


