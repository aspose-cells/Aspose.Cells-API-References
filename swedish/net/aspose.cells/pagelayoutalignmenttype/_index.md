---
title: "Enum PageLayoutAlignmentType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.PageLayoutAlignmentType‑enum. Enumererar typer av sidlayoutjustering"
type: docs
url: /sv/net/aspose.cells/pagelayoutalignmenttype/
---
## PageLayoutAlignmentType enumeration

Enumererar sidlayoutens justeringstyper.

```csharp
public enum PageLayoutAlignmentType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Bottom | `0` | Representerar nedre sidlayoutjustering. |
| Center | `1` | Representerar centrerad sidlayoutjustering. |
| Left | `2` | Representerar vänster sidlayoutjustering. |
| Right | `3` | Representerar höger sidlayoutjustering. |
| Top | `4` | Representerar övre sidlayoutjustering. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageLayoutAlignmentTypeDemo
    {
        public static void PageLayoutAlignmentTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);
            worksheet.Cells["A4"].PutValue(789);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Ange dataintervallet för diagrammet
            chart.SetChartDataRange("A1:A4", true);

            // Ange diagrammets titel
            chart.Title.Text = "Sample Chart";

            // Spara arbetsboken till en fil
            workbook.Save("PageLayoutAlignmentTypeExample.xlsx");

            // Exportera diagrammet till en PDF med specifik sidlayoutjustering
            chart.ToPdf("ChartExample.pdf", 8.5f, 11f, PageLayoutAlignmentType.Center, PageLayoutAlignmentType.Center);

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


