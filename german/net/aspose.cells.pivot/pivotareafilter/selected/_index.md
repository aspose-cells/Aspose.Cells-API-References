---
title: "PivotAreaFilter.Selected"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotAreaFilter-Eigenschaft. Gibt an, ob dieses Feld eine Auswahl hat. Funktioniert nur, wenn die PivotTable in der Gliederungsansicht ist"
type: docs
url: /de/net/aspose.cells.pivot/pivotareafilter/selected/
---
## PivotAreaFilter.Selected property

Gibt an, ob dieses Feld eine Auswahl hat. Funktioniert nur, wenn die PivotTable in der Gliederungsansicht ist.

```csharp
public bool Selected { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaFilterPropertySelectedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Erstelle eine Pivot-Tabelle
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Hole Pivotbereich-Filter
            PivotArea pivotArea = new PivotArea(pivotTable);
            PivotAreaFilter filter = pivotArea.Filters[0];

            // Zeige den aktuellen ausgewählten Wert an
            Console.WriteLine("Current Selected value: " + filter.Selected);

            // Ausgewählten Wert ändern (betrifft nur die Gliederungsansicht)
            filter.Selected = true;
            Console.WriteLine("New Selected value: " + filter.Selected);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotAreaFilterSelectedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


