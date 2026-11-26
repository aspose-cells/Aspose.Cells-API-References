---
title: "Top10.Rank"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Top10. Obtener o establecer el valor de n en una regla de formato condicional top/bottom n. Si IsPercent es verdadero, el valor debe estar entre 0 y 100. De lo contrario, debe estar entre 0 y 1000. El valor predeterminado es 10"
type: docs
url: /es/net/aspose.cells/top10/rank/
---
## Top10.Rank property

Obtener o establecer el valor de "n" en una regla de formato condicional "top/bottom n". Si IsPercent es true, el valor debe estar entre 0 y 100. De lo contrario debe estar entre 0 y 1000. El valor predeterminado es 10.

```csharp
public int Rank { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class Top10PropertyRankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            Top10 top10 = fc.Top10;
            top10.Rank = 5;

            workbook.Save("Top10RankExample.xlsx");
        }
    }
}
```

### Ver también

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


