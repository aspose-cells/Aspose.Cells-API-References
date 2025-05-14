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
         //http://www.aspose.com/community/forums/thread/338075/how-to-set-color-to-category-axis.aspx
         public void Axis_Property_Area()
         {
             Console.WriteLine("testCELLSNET_40009()");
             string infn = path + @"example.xlsm";
             string outfn = destpath + @"tmp.out.xlsm";

             Workbook wb = new Workbook(infn);
             Console.WriteLine(wb.Worksheets[0].Charts[0].CategoryAxis.Area.BackgroundColor);
             wb.Save(outfn);
#if WTEST
            Process.Start("explorer.exe", string.Format("\"{0}\"", outfn));
#endif
         }
```

### See Also

* class [Area](../../../aspose.cells.drawing/area/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


