---
title: Chart.Perspective
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Returns or sets the perspective for the 3D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True
type: docs
url: /net/aspose.cells.charts/chart/perspective/
---
## Chart.Perspective property

Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True.

```csharp
public short Perspective { get; set; }
```

### Examples

```csharp
// Called: charts[0].Perspective = 0;
[Ignore]
#endif
        // How to change 2d contour color fill or palette in XlsIO
        // http://www.aspose.com/community/forums/thread/290821.aspx
        public void Property_Perspective()
        {
            Console.WriteLine(&quot;Property_Perspective()&quot;);
            string infn = path + @&quot;CELLSNET-25239\SurfaceContour+Chart.xls&quot;;
            string outfn = Constants.destPath + @&quot;CELLSNET-25239.xlsx&quot;;

            Workbook w = new Workbook(infn);
            //w.CalculateFormula();
            //Console.Out.Write(w.Worksheets[&quot;NGERS_DCA_SUMMARY&quot;].Cells[&quot;D22&quot;].StringValue);
            //HtmlSaveOptions options = new HtmlSaveOptions();
            //options.DisplayHTMLCrossString = true;
            //w.Save(@&quot;D:\FileTemp\dest.html&quot;, options);
            //SpreadsheetML2003SaveOptions s = new SpreadsheetML2003SaveOptions();
            //s.LimitAsXls = false;
            //w.Save(@&quot;D:\FileTemp\dest.xml&quot;,s);
            int x = w.Worksheets.Add(SheetType.Chart);
            Aspose.Cells.Charts.ChartCollection charts = w.Worksheets[x].Charts;
            charts.Add(Aspose.Cells.Charts.ChartType.Surface3D, 0, 0, 10, 10);
            charts[0].NSeries.Add(&quot;&apos;Temperature, Field_data&apos;!B2:U21&quot;, false);
            for (int i = 0; i &lt; charts[0].NSeries.Count; i++)
            {
                charts[0].NSeries[i].Name = &quot;=&apos;Temperature, Field_data&apos;!A&quot; + (i + 2);
            }
            charts[0].NSeries.CategoryData = &quot;=&apos;Temperature, Field_data&apos;!B1:U1&quot;;
            charts[0].Perspective = 0;

            w.Save(outfn, SaveFormat.Xlsx);
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


