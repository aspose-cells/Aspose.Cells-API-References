---
title: "DataBarBorder.Color"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataBarBorder‑Eigenschaft. Gibt die Rahmenfarbe von Datenbalken zurück oder setzt sie, die durch eine bedingte Formatierungsregel festgelegt sind"
type: docs
url: /de/net/aspose.cells/databarborder/color/
---
## DataBarBorder.Color property

Liest oder setzt die Farbe der Grenze der Datenbalken, die durch eine bedingte Formatierungsregel festgelegt sind.

```csharp
public Color Color { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarBorderPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Eine Formatbedingungs‑Sammlung erstellen
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            conds.AddArea(new CellArea { StartRow = 2, StartColumn = 4, EndRow = 3, EndColumn = 6 });

            // Datenbalken‑Formatbedingung hinzufügen
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Datenbalken-Eigenschaften festlegen
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            // Rahmen‑Eigenschaften festlegen (Verwendung von Color demonstrieren)
            cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            cond.DataBar.BarBorder.Color = Color.Plum;

            // Speichere die Arbeitsmappe
            workbook.Save("DataBarBorderColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBar border color demo completed.");
        }
    }
}
```

### Siehe auch

* class [DataBarBorder](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


