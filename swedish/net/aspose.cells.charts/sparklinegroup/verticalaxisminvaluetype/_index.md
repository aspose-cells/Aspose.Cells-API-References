---
title: "SparklineGroup.VerticalAxisMinValueType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup-egenskap. Representerar den vertikala axelns minimivärdestyp"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/verticalaxisminvaluetype/
---
## SparklineGroup.VerticalAxisMinValueType property

Representerar den vertikala axelns minimivärdetyp.

```csharp
public SparklineAxisMinMaxType VerticalAxisMinValueType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMinValueTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och ett kalkylblad
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Definiera sparkline-plats
            CellArea cellArea = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Lägg till sparkline-grupp
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Ange typ för minimivärde på vertikal axel
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.AutoIndividual;

            // Spara arbetsboken
            workbook.Save("SparklineVerticalAxisMinValueTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [SparklineAxisMinMaxType](../../sparklineaxisminmaxtype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


