---
title: "PivotFieldSortSetting.LineTypeSortedBy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFieldSortSetting-Property. Der Pivot-Linientyp, nach dem sortiert wird"
type: docs
url: /de/net/aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/
---
## PivotFieldSortSetting.LineTypeSortedBy property

Der Pivot-Zeilentyp, nach dem sortiert wird.

```csharp
public PivotLineType LineTypeSortedBy { get; }
```

### Hinweise

Funktioniert nur, wenn dieses Feld nicht nach Labels sortiert wird.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldSortSettingPropertyLineTypeSortedByDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 5;

            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Sortiere in aufsteigender Reihenfolge mit Linientyp – übergebe einen leeren String für den cellName-Parameter
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.GrandTotal, "");
            
            // Demonstriere das LineTypeSortedBy-Property
            Console.WriteLine("LineTypeSortedBy: " + pivotTable.RowFields[0].SortSetting.LineTypeSortedBy);
            
            // Sortierung ändern, um den regulären Zeilentyp zu verwenden
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "C5");
            Console.WriteLine("LineTypeSortedBy after change: " + pivotTable.RowFields[0].SortSetting.LineTypeSortedBy);
        }
    }
}
```

### Siehe auch

* enum [PivotLineType](../../pivotlinetype/)
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


