---
title: Axis.MajorUnit
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the major units for the axis
type: docs
url: /net/aspose.cells.charts/axis/majorunit/
---
## Axis.MajorUnit property

Represents the major units for the axis.

```csharp
public double MajorUnit { get; set; }
```

### Remarks

The major units must be greater than zero.

### Examples

```csharp
// Called: axis.MajorUnit = 91;
public void Axis_Property_MajorUnit()
{
    var workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    //    workbook.Save(workbook.FileName + "_out.pdf");
    var chart = workbook.Worksheets[0].Charts[0];
    chart.Calculate();
    // chart.ToImage(dir + "a.png");return;
    var axis = chart.CategoryAxis;
    Console.WriteLine(axis.GetAxisTexts().Length); // ISSUE #1: incorrectly returned 27 where it was only 13

    // changing the major unit to reduce the tickmarks to 5 (equivalent in the gif doing in MS Excel attached)
    //axis.CategoryType = CategoryType.TimeScale;
    axis.MajorUnitScale = TimeUnit.Days;
    axis.MajorUnit = 91;
    chart.Calculate();
    Console.WriteLine(axis.GetAxisTexts().Length); // correctly returned 5
                                              // Convert the chart to an image file.
    workbook.Save(Constants.destPath + "example.xlsx"); // ISSUE #2: the number of tickmarks in the document is not actually changed (13)
    var wb2 = new Workbook(Constants.destPath + "example.xlsx");
    chart = wb2.Worksheets[0].Charts[0];
    Assert.AreEqual(chart.CategoryAxis.MajorUnitScale, TimeUnit.Days, "Major Unit Scale");
    Assert.AreEqual(chart.CategoryAxis.MajorUnit, 91, "Major Unit");
    //wb2.Worksheets[0].Charts[0].ToImage(wb2.FileName + @"_out2.emf", ImageFormat.Emf);//// ISSUE #3 if I convert the chart to image using Aspose.Cells, more tickmarks are present in the image (27   }

}
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


