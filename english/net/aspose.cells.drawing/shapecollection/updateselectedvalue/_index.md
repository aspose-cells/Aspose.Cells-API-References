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
// Called: worksheet.Shapes.UpdateSelectedValue();
[Test]
        public void Method_UpdateSelectedValue()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;Cellsjava42352.xlsx&quot;);
            Worksheet worksheet = wb.Worksheets[0];
            worksheet.Cells[&quot;B2&quot;].Value = (321);
            worksheet.Shapes.UpdateSelectedValue();
            Assert.AreEqual(worksheet.Shapes[0].Text, &quot;321&quot;);
            Assert.AreEqual(worksheet.Shapes[1].Text, &quot;321&quot;);
            wb.Save(Constants.destPath + &quot;112.html&quot;);
        }
```

### See Also

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


