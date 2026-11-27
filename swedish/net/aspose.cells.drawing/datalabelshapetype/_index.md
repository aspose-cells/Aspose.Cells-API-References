---
title: "Enum DataLabelShapeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.DataLabelShapeType-enum. Anger den förinställda formgeometrin som ska användas för ett diagram"
type: docs
url: /sv/net/aspose.cells.drawing/datalabelshapetype/
---
## DataLabelShapeType enumeration

Specificerar den förinställda formgeometrin som ska användas för ett diagram.

```csharp
public enum DataLabelShapeType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Rect | `0` | Representerar rektangelformen. |
| RoundRect | `1` | Representerar den rundade rektangelformen. |
| Ellipse | `2` | Representerar ellipsformen. |
| RightArrowCallout | `3` | Representerar den högra pilpointerns form. |
| DownArrowCallout | `4` | Representerar den nedåtpilpointerns form. |
| LeftArrowCallout | `5` | Representerar den vänstra pilpointerns form. |
| UpArrowCallout | `6` | Representerar den uppåtpilpointerns form. |
| WedgeRectCallout | `7` | Representerar den kilrektangel-pointerns form. |
| WedgeRoundRectCallout | `8` | Representerar den kilrunda rektangel-pointerns form. |
| WedgeEllipseCallout | `9` | Representerar den kilellips-pointerns form. |
| LineCallout | `10` | Representerar linjekalloutformen. |
| BentLineCallout | `11` | Representerar den böjda linjekalloutformen. |
| LineWithAccentBarCallout | `12` | Representerar linjen med accentstapelkalloutformen. |
| BentLineWithAccentBarCallout | `13` | Representerar den böjda linjen med accentstapelkalloutformen. |
| Line | `14` | Denna typ används endast för speciell filbehandling. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class DataLabelShapeTypeDemo
    {
        public static void DataLabelShapeTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataintervall
            chart.SetChartDataRange("A1:B4", true);

            // Få åtkomst till den första serien i diagrammet
            Series series = chart.NSeries[0];

            // Aktivera datamärkningar för serien.
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShapeType = DataLabelShapeType.RoundRect;

            // Spara arbetsboken
            workbook.Save("DataLabelShapeTypeExample.xlsx");
            workbook.Save("DataLabelShapeTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


