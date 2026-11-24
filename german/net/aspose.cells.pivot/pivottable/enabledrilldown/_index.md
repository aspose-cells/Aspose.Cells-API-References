---
title: "PivotTable.EnableDrilldown"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob Drilldown aktiviert ist"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/enabledrilldown/
---
## PivotTable.EnableDrilldown property

Gibt an, ob Drilldown aktiviert ist.

```csharp
public bool EnableDrilldown { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableDrilldownDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ein Arbeitsblatt hinzufügen und mit Beispieldaten füllen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Erstelle eine Pivot-Tabelle
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Konfiguriere PivotTable-Felder
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Drilldown-Funktionalität aktivieren
            pivotTable.EnableDrilldown = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableEnableDrilldownDemo.xlsx");
            
            // Überprüfen, ob die Eigenschaft gesetzt wurde
            Console.WriteLine("EnableDrilldown property is set to: " + pivotTable.EnableDrilldown);
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


