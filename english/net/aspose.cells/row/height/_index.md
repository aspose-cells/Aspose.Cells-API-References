---
title: Row.Height
second_title: Aspose.Cells for .NET API Reference
description: Row property. Gets and sets the row height in unit of Points
type: docs
url: /net/aspose.cells/row/height/
---
## Row.Height property

Gets and sets the row height in unit of Points.

```csharp
public double Height { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(99.95, row.Height, "Row height of 5(A5's value is testing)=");
[Test]
        public void Property_Height()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "SSML\\CellsNet43184.xml");
            Row row = workbook.Worksheets[0].Cells.Rows[4];
            Assert.AreEqual(99.95, row.Height, "Row height of 5(A5's value is testing)=");
            Assert.IsFalse(row.IsHeightMatched, "Row.IsHeightMatched");
        }
```

### See Also

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


