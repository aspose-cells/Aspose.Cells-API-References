---
title: Chart.Style
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets and sets the builtin style
type: docs
url: /net/aspose.cells.charts/chart/style/
---
## Chart.Style property

Gets and sets the builtin style.

```csharp
public int Style { get; set; }
```

### Remarks

It should be between 1 and 48. Return -1 if it's not be set.

### Examples

```csharp
// Called: ch.Style = sh.Charts[0].Style;
[Test]
         //http://www.aspose.com/community/forums/thread/344750/copying-charts.aspx
         public void Property_Style()
         {
             Console.WriteLine(&quot;testCELLSNET_40128()&quot;);
             string infn = path + @&quot;CELLSNET-40128\Book1_40128.xlsx&quot;;
             string outfn = destpath + @&quot;Book1_40128.out.png&quot;;
             string outfn1 = destpath + @&quot;Book1_40128.out.xlsx&quot;;

             Workbook wb1 = new Workbook(infn);
             Workbook wb2 = new Workbook();
             Worksheet sh = wb1.Worksheets[&quot;Sheet1&quot;];
             wb2.Worksheets.Add();
             wb2.Worksheets[0].Copy(sh);

             sh = wb1.Worksheets[&quot;Chart1&quot;];
             wb2.Worksheets.Add();
             Int32 i = 1;
             wb2.Worksheets[i].Copy(sh);
             Aspose.Cells.Charts.Chart ch = wb2.Worksheets[i].Charts[0];
             ch.NSeries.Clear();
             ch.NSeries.Add(&quot;Sheet1!B2:C3&quot;, false);
             ch.NSeries.CategoryData = &quot;Sheet1!B1:C1&quot;;
             ch.Style = sh.Charts[0].Style;
             for (int j = 0; j &lt; ch.NSeries.Count; j++)
             {
                 ch.NSeries[j].Name = &quot;=Sheet1!&quot; + CellsHelper.CellIndexToName(1 + j, 0);
             }
             wb2.Save(outfn1);
             wb2.Worksheets[1].Charts[0].ToImage(outfn);
#if WTEST
             Process.Start(&quot;explorer.exe&quot;, string.Format(&quot;\&quot;{0}\&quot;&quot;, outfn));
#endif
         }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


