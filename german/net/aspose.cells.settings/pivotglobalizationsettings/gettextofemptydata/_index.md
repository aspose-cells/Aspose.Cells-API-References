---
title: "PivotGlobalizationSettings.GetTextOfEmptyData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotGlobalizationSettings-Methode. Gibt den Text des leeren Etiketts in der PivotTable zurück"
type: docs
url: /de/net/aspose.cells.settings/pivotglobalizationsettings/gettextofemptydata/
---
## PivotGlobalizationSettings.GetTextOfEmptyData method

Ermittelt den Text der Beschriftung "(blank)" in der PivotTable.

```csharp
public virtual string GetTextOfEmptyData()
```

### Rückgabewert

Der Text für leere Daten

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfEmptyDataDemo
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
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1500);

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Erstellen und verwenden Sie PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Demonstrieren Sie die Methode GetTextOfEmptyData
            Console.WriteLine("Empty Data Text: " + globalizationSettings.GetTextOfEmptyData());

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


