---
title: Worksheet.Shapes
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Returns all drawing shapes in this worksheet
type: docs
url: /net/aspose.cells/worksheet/shapes/
---
## Worksheet.Shapes property

Returns all drawing shapes in this worksheet.

```csharp
public ShapeCollection Shapes { get; }
```

### Examples

```csharp
// Called: sheet.Shapes.AddAutoShape(AutoShapeType.Octagon, 1, 1, 5, 5, 50, 50);
[Test]
        public void Property_Shapes()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Name = "Octagon";
            sheet.Shapes.AddAutoShape(AutoShapeType.Octagon, 1, 1, 5, 5, 50, 50);

            checkAutoShapeType_Octagon(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkAutoShapeType_Octagon(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkAutoShapeType_Octagon(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


