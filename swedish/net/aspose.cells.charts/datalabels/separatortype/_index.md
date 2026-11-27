---
title: "DataLabels.SeparatorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Hämtar eller anger separator-typen som används för dataetiketterna på ett diagram"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/separatortype/
---
## DataLabels.SeparatorType property

Hämtar eller anger separatorns typ som används för datamärken i ett diagram.

```csharp
public DataLabelsSeparatorType SeparatorType { get; set; }
```

### Anmärkningar

För att ange en anpassad separator, vänligen sätt egenskapen `SeparatorType` till Custom och ange sedan det förväntade värdet för [`SeparatorValue`](../separatorvalue/).

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertySeparatorTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Aktivera datamärkningar
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.ShowCategoryName = true;
            
            // Ange separator-typ
            chart.NSeries[0].DataLabels.SeparatorType = DataLabelsSeparatorType.Space;

            // Spara arbetsboken
            workbook.Save("DataLabelsSeparatorTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [DataLabelsSeparatorType](../../datalabelsseparatortype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


