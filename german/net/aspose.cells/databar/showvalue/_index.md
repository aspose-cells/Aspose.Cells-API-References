---
title: "DataBar.ShowValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataBar-Eigenschaft. Gibt das Flag zurück oder legt es fest, das angibt, ob die Werte der Zellen angezeigt werden sollen, auf die dieser Datenbalken angewendet wird. Standardwert ist true"
type: docs
url: /de/net/aspose.cells/databar/showvalue/
---
## DataBar.ShowValue property

Lese oder setze das Flag, das angibt, ob die Werte der Zellen angezeigt werden sollen, auf die dieser Datenbalken angewendet wird. Der Standardwert ist true.

```csharp
public bool ShowValue { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyShowValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Bedingte Formatierung für Datenbalken hinzufügen
            int idx = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Datenbalken-Bedingung hinzufügen
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];
            
            // Datenbalken-Eigenschaften festlegen
            fc.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            fc.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.DataBar.Color = Color.Green;
            
            // ShowValue-Eigenschaft demonstrieren
            fc.DataBar.ShowValue = true; // Show cell values along with data bars
            
            // Speichere die Arbeitsmappe
            workbook.Save("DataBarShowValueDemo.xlsx");
            
            Console.WriteLine("DataBar ShowValue demo completed. Output file: DataBarShowValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


