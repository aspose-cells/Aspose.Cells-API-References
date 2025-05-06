---
title: Series.LeaderLines
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents leader lines on a chart. Leader lines connect data labels to data points. This object isnt a collection theres no object that represents a single leader line
type: docs
url: /net/aspose.cells.charts/series/leaderlines/
---
## Series.LeaderLines property

Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn’t a collection; there’s no object that represents a single leader line.

```csharp
public Line LeaderLines { get; }
```

### Examples

```csharp
// Called: ser.LeaderLines.Style = LineType.Dot;
[Test]
        //http://www.aspose.com/community/forums/thread/223686.aspx
        public void Property_LeaderLines()
        {
            Console.WriteLine(&quot;Property_LeaderLines()&quot;);
            string infn = path + &quot;Test_ASeriesLeadLines.xlsx&quot;;
            string outfn = Constants.destPath + &quot;Test_ASeriesLeadLines_out.xlsx&quot;;

            Workbook book = new Workbook(infn);
            Chart c = book.Worksheets[0].Charts[0];

            Series ser = c.NSeries[0];
            ser.DataLabels.ShowCategoryName = true;
            ser.DataLabels.ShowPercentage = true;
            ser.DataLabels.TextFont.Name = &quot;Arial&quot;;
            ser.DataLabels.TextFont.Size = 12;
            ser.DataLabels.TextFont.IsBold = true;
            ser.DataLabels.Position = LabelPositionType.BestFit;
            //ser.HasLeaderLines = true;
            ser.LeaderLines.IsAuto = false;
            ser.LeaderLines.Style = LineType.Dot;
            ser.LeaderLines.WeightPt = 0.25;
            ser.LeaderLines.Color = Color.LightCyan;

            book.Save(outfn);
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


