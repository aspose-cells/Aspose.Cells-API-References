---
title: Area.Transparency
second_title: Aspose.Cells for .NET API Reference
description: Area property. Returns or sets the degree of transparency of the area as a value from 0.0 opaque through 1.0 clear
type: docs
url: /net/aspose.cells.drawing/area/transparency/
---
## Area.Transparency property

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```csharp
public double Transparency { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine("area trans: " + ser.Area.Transparency);
//http://www.aspose.com/community/forums/thread/224730.aspx
public void Area_Property_Transparency()
{
    Console.WriteLine("Area_Property_Transparency()");
    string infn = path + "Test_SimpleTransparency.xlsx";
    string outfn = Constants.destPath + "Test_SimpleTransparency_out.xlsx";

    Workbook book = new Workbook(infn);
    Chart c = book.Worksheets[0].Charts[0];
    Series ser = c.NSeries[0];
    Console.WriteLine("area trans: " + ser.Area.Transparency);
    Console.WriteLine("line trans: " + ser.Border.Transparency);
    ser.Area.Transparency = .8;
    ser.Border.Transparency = 0;
    book.Save(outfn);
}
```

### See Also

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


