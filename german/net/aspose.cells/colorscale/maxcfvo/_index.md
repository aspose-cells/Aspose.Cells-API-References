---
title: "ColorScale.MaxCfvo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ColorScale-Eigenschaft. Abrufen oder Festlegen dieses Maximalwertobjekts der ColorScales. Null oder ein CFValueObject mit dem Typ FormatConditionValueType.Min kann nicht gesetzt werden."
type: docs
url: /de/net/aspose.cells/colorscale/maxcfvo/
---
## ColorScale.MaxCfvo property

Lese oder setze das Maximalwert‑Objekt dieser ColorScale. Es kann nicht null oder ein CFValueObject mit dem Typ FormatConditionValueType.Min zugewiesen werden.

```csharp
public ConditionalFormattingValue MaxCfvo { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMaxCfvoDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            ws.Cells["A1"].PutValue(1);
            ws.Cells["A2"].PutValue(2);
            ws.Cells["A3"].PutValue(3);
            ws.Cells["A4"].PutValue(4);
            ws.Cells["A5"].PutValue(5);

            int idx = ws.ConditionalFormattings.Add();
            FormatConditionCollection fcc = ws.ConditionalFormattings[idx];
            fcc.AddArea(CellArea.CreateCellArea("A1", "A5"));

            idx = fcc.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcc[idx];
            
            fc.ColorScale.Is3ColorScale = false;
            
            // Demonstriere die Verwendung der MaxCfvo‑Eigenschaft
            fc.ColorScale.MaxCfvo.IsGTE = true;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Yellow;
            
            fc.ColorScale.MinCfvo.IsGTE = true;
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;

            workbook.Save("ColorScaleMaxCfvoDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


