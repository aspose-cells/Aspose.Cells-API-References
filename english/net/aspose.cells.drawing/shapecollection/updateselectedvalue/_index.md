---
title: ShapeCollection.UpdateSelectedValue
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Update the selected value by the value of the linked cell or range of the shape
type: docs
url: /net/aspose.cells.drawing/shapecollection/updateselectedvalue/
---
## ShapeCollection.UpdateSelectedValue method

Update the selected value by the value of the linked cell or range of the shape.

```csharp
public void UpdateSelectedValue()
```

### Examples

```csharp
// Called: sheet.Shapes.UpdateSelectedValue();
[Test]
        public void Method_UpdateSelectedValue()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA-41731.xls");
            Worksheet sheet = workbook.Worksheets[2];
            sheet.Cells["M10"].PutValue("Opps!");

            workbook.CalculateFormula();
            sheet.Shapes.UpdateSelectedValue();
            Assert.AreEqual(sheet.Shapes[0].TextEffect.Text, "Opps!");
           
        }
```

### See Also

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


