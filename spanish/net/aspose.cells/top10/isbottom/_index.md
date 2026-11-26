---
title: "Top10.IsBottom"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Top10. Obtiene o establece si una regla superior/inferior n es una regla inferior n. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/top10/isbottom/
---
## Top10.IsBottom property

Obtener o establecer si una regla "top/bottom n" es una regla "bottom n". El valor predeterminado es false.

```csharp
public bool IsBottom { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class Top10PropertyIsBottomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i + 1);
            }

            // Agregar formato condicional
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            fcs.AddArea(new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 0 });

            // Agregar condición Top10
            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Configurar propiedades Top10
            Top10 top10 = fc.Top10;
            top10.IsBottom = true; // Highlight bottom values
            top10.IsPercent = false;
            top10.Rank = 3; // Highlight bottom 3 values

            workbook.Save("Top10IsBottomExample.xlsx");
        }
    }
}
```

### Ver también

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


