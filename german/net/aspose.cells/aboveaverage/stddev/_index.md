---
title: "AboveAverage.StdDev"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AboveAverage-Eigenschaft. Gibt die Anzahl der Standardabweichungen an, die über oder unter dem Durchschnitt in der bedingten Formatierungsregel einbezogen werden sollen, oder legt sie fest. Der Eingabewert muss zwischen 0 und 3 liegen, einschließlich 0 und 3. Das Setzen dieses Wertes auf 0 bedeutet, dass stdDev nicht gesetzt ist. Der Standardwert ist 0"
type: docs
url: /de/net/aspose.cells/aboveaverage/stddev/
---
## AboveAverage.StdDev property

Lese oder setze die Anzahl der Standardabweichungen, die über oder unter dem Durchschnitt in der bedingten Formatierungsregel berücksichtigt werden sollen. Der Eingabewert muss zwischen 0 und 3 liegen (inklusive 0 und 3). Wird dieser Wert auf 0 gesetzt, ist stdDev nicht festgelegt. Der Standardwert ist 0.

```csharp
public int StdDev { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyStdDevDemo
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
            fc.Style.BackgroundColor = Color.Yellow;

            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.StdDev = 2;

            // Beispieldaten befüllen
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            worksheet.Cells["A4"].Value = 40;
            worksheet.Cells["A5"].Value = 50;

            workbook.Save("AboveAverageStdDevDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


