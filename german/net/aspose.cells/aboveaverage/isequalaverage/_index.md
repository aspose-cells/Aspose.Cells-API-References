---
title: "AboveAverage.IsEqualAverage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AboveAverage-Eigenschaft. Gibt das Flag an oder legt es fest, das angibt, ob die aboveAverage- und belowAverage-Kriterien den Durchschnitt selbst einschließen oder von diesem Wert ausschließen. true bedeutet, den Durchschnittswert in die Kriterien einzuschließen. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/aboveaverage/isequalaverage/
---
## AboveAverage.IsEqualAverage property

Lese oder setze das Flag, das angibt, ob die Kriterien 'aboveAverage' und 'belowAverage' den Durchschnittswert einschließen oder ausschließen. 'true' bedeutet, den Durchschnittswert in die Kriterien einzubeziehen. Standardwert ist false.

```csharp
public bool IsEqualAverage { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyIsEqualAverageDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.LightBlue;

            // Demonstriere die IsEqualAverage-Eigenschaft
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false; // Cells equal to average won't be formatted

            // Beispieldaten befüllen
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            worksheet.Cells["A4"].Value = 40;
            worksheet.Cells["A5"].Value = 50; // Average is 30

            workbook.Save("AboveAverageIsEqualAverageDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


