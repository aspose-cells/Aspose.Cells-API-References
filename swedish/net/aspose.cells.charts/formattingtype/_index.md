---
title: "Enum FormattingType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.FormattingType enum. Representerar typen av formatering som tillämpas på ett Area-objekt eller ett Line-objekt"
type: docs
url: /sv/net/aspose.cells.charts/formattingtype/
---
## FormattingType enumeration

Representerar typen av formatering som tillämpas på ett [`Area`](../../aspose.cells.drawing/area/) objekt eller ett [`Line`](../../aspose.cells.drawing/line/) objekt.

```csharp
public enum FormattingType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Automatic | `0` | Representerar automatisk formateringstyp. |
| Custom | `2` | Representerar anpassad formateringstyp. |
| None | `1` | Representerar ingen formateringstyp. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class FormattingTypeDemo
    {
        public static void FormattingTypeExample()
        {
            // Instansiera ett Workbook-objekt
            Workbook workbook = new Workbook();
            
            // Lägga till ett nytt kalkylblad i Workbook-objektet
            int sheetIndex = workbook.Worksheets.Add();
            
            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Lägger till exempelvärden i celler
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Lägger till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Åtkomst till instansen av det nyligen tillagda diagrammet
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägger till NSeries (diagramdatakälla) till diagrammet som sträcker sig från cellen "A1" till "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Ställer in förgrundsfärgen för plotområdet
            chart.PlotArea.Area.ForegroundColor = Color.Blue;
            chart.PlotArea.Area.Formatting = FormattingType.Custom;
            
            // Ställer in förgrundsfärgen för diagramområdet
            chart.ChartArea.Area.ForegroundColor = Color.Yellow;
            chart.ChartArea.Area.Formatting = FormattingType.Automatic;
            
            // Ställer in förgrundsfärgen för det första NSeries-området
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.Formatting = FormattingType.None;
            
            // Ställer in förgrundsfärgen för området för den första NSeries-punkten
            chart.NSeries[0].Points[0].Area.ForegroundColor = Color.Cyan;
            chart.NSeries[0].Points[0].Area.Formatting = FormattingType.Custom;
            
            // Sparar Excel-filen
            workbook.Save("FormattingTypeExample.xlsx");
            workbook.Save("FormattingTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


