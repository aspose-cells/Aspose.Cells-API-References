---
title: Line.WeightPt
second_title: Aspose.Cells for .NET API Reference
description: Line property. Gets or sets the weight of the line in unit of points
type: docs
url: /net/aspose.cells.drawing/line/weightpt/
---
## Line.WeightPt property

Gets or sets the weight of the line in unit of points.

```csharp
public double WeightPt { get; set; }
```

### Examples

```csharp
// Called: ser.LeaderLines.WeightPt = 0.25;
[Test]
        //http://www.aspose.com/community/forums/thread/223686.aspx
        public void Property_WeightPt()
        {
            Console.WriteLine("Property_WeightPt()");
            string infn = path + "Test_ASeriesLeadLines.xlsx";
            string outfn = Constants.destPath + "Test_ASeriesLeadLines_out.xlsx";

            Workbook book = new Workbook(infn);
            Chart c = book.Worksheets[0].Charts[0];

            Series ser = c.NSeries[0];
            ser.DataLabels.ShowCategoryName = true;
            ser.DataLabels.ShowPercentage = true;
            ser.DataLabels.TextFont.Name = "Arial";
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


