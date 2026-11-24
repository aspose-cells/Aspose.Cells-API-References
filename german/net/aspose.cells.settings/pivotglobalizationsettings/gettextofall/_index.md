---
title: "PivotGlobalizationSettings.GetTextOfAll"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotGlobalizationSettings-Methode. Gibt den Text des All‑Labels in der PivotTable zurück"
type: docs
url: /de/net/aspose.cells.settings/pivotglobalizationsettings/gettextofall/
---
## PivotGlobalizationSettings.GetTextOfAll method

Ermittelt den Text der Beschriftung "(All)" in der PivotTable.

```csharp
public virtual string GetTextOfAll()
```

### Rückgabewert

Der Text der "(All)"‑Beschriftung

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfAllDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Globalisierungseinstellungen erstellen und verwenden
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Demonstriere die Methode GetTextOfAll
            Console.WriteLine("Text of All: " + globalizationSettings.GetTextOfAll());

            // Speichere die Arbeitsmappe
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


