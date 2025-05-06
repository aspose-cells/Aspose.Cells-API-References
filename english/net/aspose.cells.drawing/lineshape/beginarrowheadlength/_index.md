---
title: LineShape.BeginArrowheadLength
second_title: Aspose.Cells for .NET API Reference
description: LineShape property. Gets and sets the begin arrow head length of the line
type: docs
url: /net/aspose.cells.drawing/lineshape/beginarrowheadlength/
---
## LineShape.BeginArrowheadLength property

Gets and sets the begin arrow head length of the line.

```csharp
[Obsolete("Use Shape.Line.BeginArrowheadLength property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoArrowheadLength BeginArrowheadLength { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use Shape.Line.BeginArrowheadLength property. This property will be removed 12 months later since August 2016. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: line2.BeginArrowheadLength = MsoArrowheadLength.Medium;
[Test]
          public void Property_BeginArrowheadLength()
          {
              var wb = new Workbook();
              var sheet0 = wb.Worksheets[0];

              // Add a line to the worksheet 
              Aspose.Cells.Drawing.LineShape line2 = sheet0.Shapes.AddLine(7, 0, 1, 0, 85, 250);
              // Set the line color 
              line2.Line.FillType = FillType.Solid;
              line2.Line.SolidFill.Color = Color.Red;
              // Set the weight of the line. 
              line2.Line.Weight = 3;
              // Set the placement. 
              line2.Placement = PlacementType.FreeFloating;
              // Set the line arrows. 
              line2.EndArrowheadWidth = MsoArrowheadWidth.Medium;
              line2.EndArrowheadStyle = MsoArrowheadStyle.Arrow;
              line2.EndArrowheadLength = MsoArrowheadLength.Medium;
              line2.BeginArrowheadStyle = MsoArrowheadStyle.ArrowDiamond;
              line2.BeginArrowheadLength = MsoArrowheadLength.Medium;
              // Make the gridlines invisible in the first worksheet. 
              sheet0.IsGridlinesVisible = false;


              wb.Save(Constants.destPath + &quot;CELLSNET44696.xlsx&quot;, SaveFormat.Xlsx);
              wb = new Workbook(Constants.destPath + &quot;CELLSNET44696.xlsx&quot;);
              Shape shape = wb.Worksheets[0].Shapes[0];
              Assert.AreEqual(shape.Line.EndArrowheadWidth, MsoArrowheadWidth.Medium);
          }
```

### See Also

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


