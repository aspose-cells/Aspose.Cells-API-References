---
title: "FormatCondition.Top10"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormatCondition. Obtiene la instancia Top10 de los formatos condicionales. La regla predeterminada de la instancia resalta las celdas cuyos valores están dentro del top 10. Válido solo para el tipo Top10"
type: docs
url: /es/net/aspose.cells/formatcondition/top10/
---
## FormatCondition.Top10 property

Obtenga la instancia "Top10" del formato condicional. La regla de la instancia predeterminada resalta celdas cuyos valores están dentro del top 10. Válido solo para type = Top10.

```csharp
public Top10 Top10 { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTop10Demo
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
            top10.IsPercent = true;
            top10.IsBottom = true;
            top10.Rank = 10;

            workbook.Save("FormatConditionPropertyTop10Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Top10](../../top10/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


