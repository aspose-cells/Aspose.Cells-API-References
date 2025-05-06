---
title: Axis.Area
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Gets the Area
type: docs
url: /net/aspose.cells.charts/axis/area/
---
## Axis.Area property

Gets the `Area`.

```csharp
public Area Area { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(wb.Worksheets[0].Charts[0].CategoryAxis.Area.BackgroundColor);
[Test]
         //http://www.aspose.com/community/forums/thread/338075/how-to-set-color-to-category-axis.aspx
         public void Property_Area()
         {
             Console.WriteLine(&quot;testCELLSNET_40009()&quot;);
             string infn = path + @&quot;CELLSNET-40009\tmp.xlsm&quot;;
             string outfn = destpath + @&quot;tmp.out.xlsm&quot;;

             Workbook wb = new Workbook(infn);
             Console.WriteLine(wb.Worksheets[0].Charts[0].CategoryAxis.Area.BackgroundColor);
             wb.Save(outfn);
#if WTEST
            Process.Start(&quot;explorer.exe&quot;, string.Format(&quot;\&quot;{0}\&quot;&quot;, outfn));
#endif
         }
```

### See Also

* class [Area](../../../aspose.cells.drawing/area/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


