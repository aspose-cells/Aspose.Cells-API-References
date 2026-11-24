---
title: "PivotTable.RefreshedByWho"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt den Namen des letzten Benutzers zurück, der diese PivotTable aktualisiert hat"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/refreshedbywho/
---
## PivotTable.RefreshedByWho property

Liest den Namen des letzten Benutzers, der diese PivotTable aktualisiert hat

```csharp
public string RefreshedByWho { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshedByWhoDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 8;

            // Pivot-Tabelle erstellen
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pt = sheet.PivotTables[pivotIndex];
            
            // Felder zur Pivot-Tabelle hinzufügen
            pt.AddFieldToArea(PivotFieldType.Row, 0);
            pt.AddFieldToArea(PivotFieldType.Data, 1);
            
            // PivotTable aktualisieren, um die Eigenschaft RefreshedByWho zu setzen
            pt.RefreshData();
            pt.CalculateData();

            // Aktualisierungsinformationen ausgeben
            Console.WriteLine("Pivot Table Refresh Information:");
            Console.WriteLine("Last Refresh Date: " + pt.RefreshDate);
            Console.WriteLine("Refreshed By: " + pt.RefreshedByWho);
            
            // Speichern und neu laden, um die Persistenz der Eigenschaft zu demonstrieren
            string savePath = "PivotTableRefreshedByWhoDemo_Out.xlsx";
            wb.Save(savePath);
            
            // Laden Sie die Arbeitsmappe neu und prüfen Sie die Eigenschaft
            Workbook wb2 = new Workbook(savePath);
            PivotTable pt2 = wb2.Worksheets[0].PivotTables[0];
            Console.WriteLine("\nAfter Reload:");
            Console.WriteLine("Last Refresh Date: " + pt2.RefreshDate);
            Console.WriteLine("Refreshed By: " + pt2.RefreshedByWho);
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


