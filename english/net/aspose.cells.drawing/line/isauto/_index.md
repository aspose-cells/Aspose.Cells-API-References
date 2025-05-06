---
title: Line.IsAuto
second_title: Aspose.Cells for .NET API Reference
description: Line property. Indicates whether this line style is auto assigned
type: docs
url: /net/aspose.cells.drawing/line/isauto/
---
## Line.IsAuto property

Indicates whether this line style is auto assigned.

```csharp
public bool IsAuto { get; set; }
```

### Examples

```csharp
// Called: ser.LeaderLines.IsAuto = false;
[Test]
        //http://www.aspose.com/community/forums/thread/223686.aspx
        public void Property_IsAuto()
        {
            Console.WriteLine(&quot;Property_IsAuto()&quot;);
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

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


