---
title: "PivotTable.RowGrand"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob Gesamtsummen für Zeilen dieser Pivot-Tabelle angezeigt werden sollen"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/rowgrand/
---
## PivotTable.RowGrand property

Gibt an, ob Gesamtsummen für Zeilen dieser Pivot-Tabelle angezeigt werden sollen.

```csharp
[Obsolete("Use PivotTable.ShowRowGrandTotals property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool RowGrand { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotTable.ShowRowGrandTotals. Diese Methode wird 12 Monate später, seit Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyRowGrandDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(2000);
            
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);
            
            worksheet.Cells["A5"].PutValue("Product A");
            worksheet.Cells["B5"].PutValue("West");
            worksheet.Cells["C5"].PutValue(1500);
            
            worksheet.Cells["A6"].PutValue("Product B");
            worksheet.Cells["B6"].PutValue("North");
            worksheet.Cells["C6"].PutValue(2500);

            // Erstelle eine Pivot-Tabelle
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C6", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Anzeige des aktuellen Werts von RowGrand
            Console.WriteLine("Current RowGrand value: " + pivotTable.RowGrand);

            // Ändern der RowGrand-Eigenschaft
            pivotTable.RowGrand = false;

            // PivotTable-Daten berechnen
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTablePropertyRowGrandDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


