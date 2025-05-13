---
title: FillFormat.GradientColor1
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Returns the gradient color 1 for the specified fill
type: docs
url: /net/aspose.cells.drawing/fillformat/gradientcolor1/
---
## FillFormat.GradientColor1 property

Returns the gradient color 1 for the specified fill.

```csharp
public Color GradientColor1 { get; }
```

### Examples

```csharp
// Called: System.Drawing.Color color1 = filleFormat.GradientColor1;
public void FillFormat_Property_GradientColor1()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Chart chart = workbook.Worksheets[1].Charts[0];
    Aspose.Cells.Drawing.FillFormat filleFormat = chart.NSeries[0].Area.FillFormat;
    System.Drawing.Color color1 = filleFormat.GradientColor1;
    double degree = filleFormat.GradientDegree;
    Console.WriteLine(chart.NSeries[0].Name);
    Console.WriteLine(color1);
    Console.WriteLine(degree);
    //filleFormat.GradientDegree = 1;
    Assert.AreEqual(Math.Round(degree, 2), 0.23);
    Assert.AreEqual(color1.ToArgb() & 0xFFFFFF, 0xFF0000);

    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


