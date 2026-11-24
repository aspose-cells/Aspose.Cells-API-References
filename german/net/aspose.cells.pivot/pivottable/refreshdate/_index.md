---
title: "PivotTable.RefreshDate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt das letzte Datum und die Uhrzeit zurück, zu der die PivotTable aktualisiert wurde"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/refreshdate/
---
## PivotTable.RefreshDate property

Liest das letzte Datum und die Uhrzeit, zu der die PivotTable aktualisiert wurde.

```csharp
public DateTime RefreshDate { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshDateDemo
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

            // Fügen Sie eine Pivot-Tabelle hinzu
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pt = sheet.PivotTables[index];
            
            // Aktualisieren Sie die PivotTable, um das Aktualisierungsdatum festzulegen
            pt.RefreshData();
            pt.CalculateData();

            // Aktualisierungsdatuminformationen anzeigen
            Console.WriteLine("Pivot Table Refresh Date: " + pt.RefreshDate.ToLongDateString());
            Console.WriteLine("Refreshed By: " + pt.RefreshedByWho);

            // Speichern und neu laden, um die Persistenz zu demonstrieren
            string savePath = "PivotTableRefreshDateDemo_Out.xlsx";
            wb.Save(savePath);
            
            // Laden Sie erneut und zeigen Sie das Aktualisierungsdatum erneut an
            Workbook wb2 = new Workbook(savePath);
            PivotTable pt2 = wb2.Worksheets[0].PivotTables[0];
            Console.WriteLine("\nAfter reloading:");
            Console.WriteLine("Pivot Table Refresh Date: " + pt2.RefreshDate.ToLongDateString());
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


