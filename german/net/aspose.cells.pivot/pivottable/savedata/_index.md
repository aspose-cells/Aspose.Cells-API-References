---
title: "PivotTable.SaveData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob Daten für den PivotTable-Bericht mit der Arbeitsmappe gespeichert werden"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/savedata/
---
## PivotTable.SaveData property

Gibt an, ob Daten für den PivotTable-Bericht mit der Arbeitsmappe gespeichert werden.

```csharp
public bool SaveData { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertySaveDataDemo
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
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // PivotTable konfigurieren
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Demonstriere die SaveData-Eigenschaft
            Console.WriteLine("SaveData before setting: " + pivotTable.SaveData);
            pivotTable.SaveData = false; // Disable saving pivot data with file
            Console.WriteLine("SaveData after setting: " + pivotTable.SaveData);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTable_SaveData_Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


