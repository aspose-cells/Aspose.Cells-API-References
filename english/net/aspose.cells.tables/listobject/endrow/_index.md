---
title: ListObject.EndRow
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets the end row of the range
type: docs
url: /net/aspose.cells.tables/listobject/endrow/
---
## ListObject.EndRow property

Gets the end row of the range.

```csharp
public int EndRow { get; }
```

### Examples

```csharp
// Called: int endRow = listObject.EndRow;
[Test]
        public void Property_EndRow()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "ListObject1.xlsx");
            ListObject listObject = workbook.Worksheets[0].ListObjects[0];

            int endRow = listObject.EndRow;
            Cells cells = workbook.Worksheets[0].Cells;
            cells.InsertRows(1, 2);
            Assert.AreEqual(listObject.EndRow, endRow + 2);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


