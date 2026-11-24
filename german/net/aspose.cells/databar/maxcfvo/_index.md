---
title: "DataBar.MaxCfvo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataBar-Eigenschaft. Gibt das Maximalwert-Objekt dieser DataBar zurück oder legt es fest. Null oder ein CFValueObject vom Typ FormatConditionValueType.Min kann nicht gesetzt werden"
type: docs
url: /de/net/aspose.cells/databar/maxcfvo/
---
## DataBar.MaxCfvo property

Lese oder setze das Maximalwert-Objekt dieses Datenbalkens. Es kann nicht null oder ein CFValueObject vom Typ FormatConditionValueType.Min zugewiesen werden.

```csharp
public ConditionalFormattingValue MaxCfvo { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMaxCfvoDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Bedingte Formatierung für Datenbalken hinzufügen
            int idx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Datenbalken hinzufügen
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[conditionIndex].DataBar;

            // MaxCfvo-Wert festlegen
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            dataBar.MaxCfvo.Value = 50;

            // Speichere die Arbeitsmappe
            workbook.Save("DataBarMaxCfvoDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


