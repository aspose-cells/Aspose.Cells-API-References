---
title: FillFormat.GradientDegree
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Returns the gradient degree for the specified fill. Only applies for Excel 2007
type: docs
url: /net/aspose.cells.drawing/fillformat/gradientdegree/
---
## FillFormat.GradientDegree property

Returns the gradient degree for the specified fill. Only applies for Excel 2007.

```csharp
public double GradientDegree { get; }
```

### Remarks

Can only be a value from 0.0 (dark) through 1.0 (light).

### Examples

```csharp
// Called: double degree = filleFormat.GradientDegree;
public void FillFormat_Property_GradientDegree()
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


