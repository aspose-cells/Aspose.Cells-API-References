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
            Console.WriteLine("Property_Perspective()");
            string infn = path + @"CELLSNET-25239\SurfaceContour+Chart.xls";
            string outfn = Constants.destPath + @"CELLSNET-25239.xlsx";

            Workbook w = new Workbook(infn);
            //w.CalculateFormula();
            //Console.Out.Write(w.Worksheets["NGERS_DCA_SUMMARY"].Cells["D22"].StringValue);
            //HtmlSaveOptions options = new HtmlSaveOptions();
            //options.DisplayHTMLCrossString = true;
            //w.Save(@"D:\FileTemp\dest.html", options);
            //SpreadsheetML2003SaveOptions s = new SpreadsheetML2003SaveOptions();
            //s.LimitAsXls = false;
            //w.Save(@"D:\FileTemp\dest.xml",s);
            int x = w.Worksheets.Add(SheetType.Chart);
            Aspose.Cells.Charts.ChartCollection charts = w.Worksheets[x].Charts;
            charts.Add(Aspose.Cells.Charts.ChartType.Surface3D, 0, 0, 10, 10);
            charts[0].NSeries.Add("'Temperature, Field_data'!B2:U21", false);
            for (int i = 0; i < charts[0].NSeries.Count; i++)
            {
                charts[0].NSeries[i].Name = "='Temperature, Field_data'!A" + (i + 2);
            }
            charts[0].NSeries.CategoryData = "='Temperature, Field_data'!B1:U1";
            charts[0].Perspective = 0;

            w.Save(outfn, SaveFormat.Xlsx);
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


