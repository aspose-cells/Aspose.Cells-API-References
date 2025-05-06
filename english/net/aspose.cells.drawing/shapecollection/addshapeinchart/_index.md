---
title: ShapeCollection.AddShapeInChart
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Add a shape to chart .All unit is 1/4000 of chart area
type: docs
url: /net/aspose.cells.drawing/shapecollection/addshapeinchart/
---
## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int, byte[]) {#addshapeinchart_1}

Add a shape to chart .All unit is 1/4000 of chart area.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom, byte[] imageData)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | The drawing type. |
| placement | PlacementType | the placement type. |
| left | Int32 | In unit of 1/4000 chart area width. |
| top | Int32 | In unit of 1/4000 chart area height. |
| right | Int32 | In unit of 1/4000 chart area width. |
| bottom | Int32 | In unit of 1/4000 chart area height. |
| imageData | Byte[] | If the shape is not a picture or ole object,imageData should be null. |

### See Also

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int) {#addshapeinchart}

Add a shape to chart .All unit is 1/4000 of chart area.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | The drawing type. |
| placement | PlacementType | the placement type. |
| left | Int32 | In unit of 1/4000 chart area width. |
| top | Int32 | In unit of 1/4000 chart area height. |
| right | Int32 | In unit of 1/4000 chart area width. |
| bottom | Int32 | In unit of 1/4000 chart area height. |

### Examples

```csharp
// Called: sheet.Charts[0].Shapes.AddShapeInChart(MsoDrawingType.CheckBox,
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            int index = workbook.Worksheets.Add(SheetType.Chart);
            Worksheet sheet = workbook.Worksheets[index];
            sheet.Charts.AddFloatingChart(ChartType.Column, 0, 0, 1024, 960);
            sheet.Charts[0].NSeries.Add(&quot;{1,2,3}&quot;, false);
            sheet.Charts[0].Shapes.AddShapeInChart(MsoDrawingType.CheckBox,
                PlacementType.Move, 400, 400, 1000, 600);
            sheet.Charts[0].Shapes[0].Text = &quot;CheckBox 1&quot;;
            int width = sheet.Charts[0].Shapes[0].Width;
            workbook.Save(Constants.destPath + &quot; CELLSNET-40174.xlsx&quot;);
        }
```

### See Also

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


