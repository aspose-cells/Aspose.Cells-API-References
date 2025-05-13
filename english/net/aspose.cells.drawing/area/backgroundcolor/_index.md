---
title: Area.BackgroundColor
second_title: Aspose.Cells for .NET API Reference
description: Area property. Gets or sets the background Color of the Area
type: docs
url: /net/aspose.cells.drawing/area/backgroundcolor/
---
## Area.BackgroundColor property

Gets or sets the background Color of the [`Area`](../).

```csharp
public Color BackgroundColor { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(wb.Worksheets[0].Charts[0].CategoryAxis.Area.BackgroundColor);
         //http://www.aspose.com/community/forums/thread/338075/how-to-set-color-to-category-axis.aspx
         public void Area_Property_BackgroundColor()
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

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


