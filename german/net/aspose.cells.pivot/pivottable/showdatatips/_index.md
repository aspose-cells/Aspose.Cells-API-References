---
title: "PivotTable.ShowDataTips"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob Tooltips für PivotTable-Datenzellen angezeigt werden sollen."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/showdatatips/
---
## PivotTable.ShowDataTips property

Gibt an, ob Tooltips für PivotTable-Datenzellen angezeigt werden sollen.

```csharp
public bool ShowDataTips { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowDataTipsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ein Arbeitsblatt und einige Beispieldaten hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 20;

            // Erstelle eine Pivot-Tabelle
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // PivotTable konfigurieren
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Datenhinweise aktivieren
            pivotTable.ShowDataTips = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableWithDataTips.xlsx");
            
            Console.WriteLine("Pivot table with ShowDataTips enabled created successfully.");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


