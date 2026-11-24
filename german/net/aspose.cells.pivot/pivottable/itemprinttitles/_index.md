---
title: "PivotTable.ItemPrintTitles"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob PivotItem-Namen oben auf jeder gedruckten Seite wiederholt werden sollen"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/itemprinttitles/
---
## PivotTable.ItemPrintTitles property

Gibt an, ob PivotItem-Namen oben auf jeder gedruckten Seite wiederholt werden sollen.

```csharp
[Obsolete("Use PivotTable.RepeatItemsOnEachPrintedPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ItemPrintTitles { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die PivotTable.RepeatItemsOnEachPrintedPage-Eigenschaft. Diese Methode wird 12 Monate später, seit Oktober 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyItemPrintTitlesDemo
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
            worksheet.Cells["A5"].PutValue("Product D");
            worksheet.Cells["B5"].PutValue("West");
            worksheet.Cells["C5"].PutValue(4000);

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Den aktuellen Wert von ItemPrintTitles anzeigen
            Console.WriteLine("Current ItemPrintTitles value: " + pivotTable.ItemPrintTitles);

            // ItemPrintTitles auf true setzen (dies ist veraltet, wird aber zur Demonstration gezeigt)
            pivotTable.ItemPrintTitles = true;

            // Alternativ die nicht veraltete Eigenschaft verwenden
            pivotTable.RepeatItemsOnEachPrintedPage = true;

            // Aktualisiere und berechne die Pivot-Tabelle
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableItemPrintTitlesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


