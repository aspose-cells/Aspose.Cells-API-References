---
title: "OdsLoadOptions.RefreshPivotTables"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsLoadOptions-Eigenschaft. Gibt an, ob Pivot-Tabellen beim Laden der Datei aktualisiert werden"
type: docs
url: /de/net/aspose.cells/odsloadoptions/refreshpivottables/
---
## OdsLoadOptions.RefreshPivotTables property

Gibt an, ob Pivot‑Tabellen beim Laden der Datei aktualisiert werden.

```csharp
public bool RefreshPivotTables { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsPropertyRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispiel-Arbeitsmappe mit Pivot-Tabelle
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Fruit");
            sheet.Cells["A4"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Item");
            sheet.Cells["B2"].PutValue("Apple");
            sheet.Cells["B3"].PutValue("Orange");
            sheet.Cells["B4"].PutValue("Carrot");
            sheet.Cells["C1"].PutValue("Price");
            sheet.Cells["C2"].PutValue(2.5);
            sheet.Cells["C3"].PutValue(3.0);
            sheet.Cells["C4"].PutValue(1.5);

            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");

            // Als ODS speichern
            string odsPath = "output.ods";
            wb.Save(odsPath, SaveFormat.Ods);

            // Lade mit RefreshPivotTables aktiviert
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            loadOptions.RefreshPivotTables = true;
            Workbook wb2 = new Workbook(odsPath, loadOptions);

            // Überprüfe, ob die Pivot-Tabelle aktualisiert wurde
            Console.WriteLine("Pivot table count: " + wb2.Worksheets[0].PivotTables.Count);
        }
    }
}
```

### Siehe auch

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


