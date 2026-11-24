---
title: "Klasse PivotFieldSortSetting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotFieldSortSetting class. Stellt die Einstellung zum Sortieren von Pivot-Feldern dar."
type: docs
url: /de/net/aspose.cells.pivot/pivotfieldsortsetting/
---
## PivotFieldSortSetting class

Stellt die Einstellung für das Sortieren von Pivot-Feldern dar.

```csharp
public class PivotFieldSortSetting
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Cell](../../aspose.cells.pivot/pivotfieldsortsetting/cell/) { get; } | Sortiert nach den Werten in welcher Zeile oder Spalte. |
| [FieldIndex](../../aspose.cells.pivot/pivotfieldsortsetting/fieldindex/) { get; set; } | (**Obsolete.**) Stellt den Index des sortierten Feldes dar. -1 bedeutet, dass das PivotField nach den Beschriftungen sortiert wird, andere Werte bedeuten, dass nach dem Datenfeld sortiert wird. |
| [IsSimpleSort](../../aspose.cells.pivot/pivotfieldsortsetting/issimplesort/) { get; set; } | Gibt an, ob ein einfacher Datensortiervorgang angewendet wird. |
| [IsSortByLabels](../../aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/) { get; } | Gibt an, ob das Feld nach sich selbst oder nach dem Datenfeld sortiert werden soll. |
| [LineTypeSortedBy](../../aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/) { get; } | Der Pivot-Zeilentyp, nach dem sortiert wird. |
| [SortBy](../../aspose.cells.pivot/pivotfieldsortsetting/sortby/) { get; set; } | Stellt den Index des sortierten Feldes dar. Ein Wert von -1 bedeutet, dass nach den eigenen Werten des Pivot-Elements sortiert wird. Wenn der Wert größer oder gleich null ist, stellt er den Index des Datenfeldes im Datenbereich dar. |
| [SortType](../../aspose.cells.pivot/pivotfieldsortsetting/sorttype/) { get; set; } | Stellt die [`SortOrder`](../../aspose.cells/sortorder/) dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotFieldSortSettingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["B4"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Pivot-Feldsortiereinstellung aus der Pivot-Tabelle abrufen
            // Hinweis: Dies setzt voraus, dass die Pivot-Tabelle Sortiereinstellungen hat, auf die wir zugreifen können
            // Da wir kein neues PivotFieldSortSetting direkt erstellen können
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;
            
            // Anzeigeneigenschaften (schreibgeschützt)
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("IsSortByLabels: " + sortSetting.IsSortByLabels);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("LineTypeSortedBy: " + sortSetting.LineTypeSortedBy);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);
            Console.WriteLine("Cell: " + sortSetting.Cell);

            // Sortierung auf die Pivot-Tabelle anwenden (die eigentliche Sortierung würde über Pivot-Tabellen-Methoden erfolgen)
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Ergebnis speichern
            workbook.Save("PivotFieldSortSettingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


