---
title: "DataBar.BarBorder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataBar-Eigenschaft. Gibt ein Objekt zurück, das den Rand einer Datenleiste angibt"
type: docs
url: /de/net/aspose.cells/databar/barborder/
---
## DataBar.BarBorder property

Liest ein Objekt, das den Rand eines Datenbalkens festlegt.

```csharp
public DataBarBorder BarBorder { get; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyBarBorderDemo
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
            int conditionIdx = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIdx];

            // Datenbalken-Eigenschaften festlegen
            fc.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            fc.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            fc.DataBar.Color = Color.Blue;
            fc.DataBar.ShowValue = true;

            // Setzen Sie die Rand-Eigenschaften der Leiste fest
            fc.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            fc.DataBar.BarBorder.Color = Color.Black;

            // Speichere die Arbeitsmappe
            workbook.Save("DataBarBorderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataBarBorder](../../databarborder/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


