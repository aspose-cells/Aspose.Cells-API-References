---
title: Cells.IsRowHidden
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Checks whether a row at given index is hidden
type: docs
url: /net/aspose.cells/cells/isrowhidden/
---
## Cells.IsRowHidden method

Checks whether a row at given index is hidden.

```csharp
public bool IsRowHidden(int rowIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | row index |

### Return Value

true if the row is hidden

### Examples

```csharp
// Called: Assert.AreEqual(rowIndex == 1, cells.IsRowHidden(rowIndex), "1-Row" + (rowIndex + 1) + ".Hidden");
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "Table/TestFile.xlsx");
            Worksheet sheet = wb.Worksheets["Sheet1"];
            Cells cells = sheet.Cells;
            // parse the first cells from the rows in the A2:C5 range
            for (int rowIndex = 1; rowIndex < 5; rowIndex++)
            {
                Assert.AreEqual(rowIndex == 1, cells.IsRowHidden(rowIndex), "1-Row" + (rowIndex + 1) + ".Hidden");
                AssertHelper.AreEqual(rowIndex == 3 ? Color.Empty : Color.FromArgb(255, 220, 230, 242),
                    cells[rowIndex, 0].GetDisplayStyle().ForegroundColor,
                    "1-A" + (rowIndex + 1) + ".DisplayStyle.ForegroundColor");
            }

            wb = new Workbook(Constants.sourcePath + "Table/TestFile2.xlsx");
            sheet = wb.Worksheets["Sheet1"];
            cells = sheet.Cells;
            // parse the first cells from the rows in the A2:C5 range
            for (int rowIndex = 1; rowIndex < 5; rowIndex++)
            {
                if (cells.IsRowHidden(rowIndex))
                {
                    Assert.Fail("2-Row" + (rowIndex + 1) + " should not be hidden");
                }
                AssertHelper.AreEqual(rowIndex % 2 == 0 ? Color.Empty : Color.FromArgb(255, 220, 230, 242),
                    cells[rowIndex, 0].GetDisplayStyle().ForegroundColor,
                    "2-A" + (rowIndex + 1) + ".DisplayStyle.ForegroundColor");
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


