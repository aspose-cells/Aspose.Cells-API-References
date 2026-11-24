---
title: "DataBar.MinCfvo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataBar-Eigenschaft. Dieses Min-Wert-Objekt der DataBars abrufen oder festlegen. Es kann nicht null oder ein CFValueObject mit dem Typ FormatConditionValueType.Max zugewiesen werden"
type: docs
url: /de/net/aspose.cells/databar/mincfvo/
---
## DataBar.MinCfvo property

Lese oder setze das Minimalwert-Objekt dieses Datenbalkens. Es kann nicht null oder ein CFValueObject vom Typ FormatConditionValueType.Max zugewiesen werden.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMinCfvoDemo
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

            // Erhalte die Sammlung der bedingten Formatierung
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];

            // Eine DataBar mit MinCfvo vom Typ "Value" erstellen
            fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[0].DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MinCfvo.Value = "5"; // Minimum value for the data bar

            // Den DataBar-Bereich festlegen
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Speichere die Arbeitsmappe
            workbook.Save("DataBarMinCfvoDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


