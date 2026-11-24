---
title: "FormatCondition.DataBar"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Eigenschaft. Rufen Sie die DataBar-Instanz der bedingten Formatierung ab. Die Standardfarbe der Instanz ist blau. Nur gültig für den Typ DataBar."
type: docs
url: /de/net/aspose.cells/formatcondition/databar/
---
## FormatCondition.DataBar property

Rufen Sie die "DataBar"-Instanz der bedingten Formatierung ab. Die Farbe der Standardinstanz ist blau. Gültig nur für Typ = DataBar.

```csharp
public DataBar DataBar { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyDataBarDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Bedingte Formatierung für Datenbalken hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Legen Sie den Bereich für die bedingte Formatierung fest
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // DataBar-Bedingung hinzufügen und Eigenschaften festlegen
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = fcs[conditionIndex];
            
            // Konfigurieren Sie DataBar-Eigenschaften
            DataBar dataBar = condition.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            dataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            dataBar.Color = System.Drawing.Color.Green;

            // Speichere die Arbeitsmappe
            workbook.Save("DataBarExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataBar](../../databar/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


