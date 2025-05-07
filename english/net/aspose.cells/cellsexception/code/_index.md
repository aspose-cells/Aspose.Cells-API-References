---
title: CellsException.Code
second_title: Aspose.Cells for .NET API Reference
description: CellsException property. Represents custom exception code
type: docs
url: /net/aspose.cells/cellsexception/code/
---
## CellsException.Code property

Represents custom exception code.

```csharp
public ExceptionType Code { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(ExceptionType.Limitation, e.Code, "Exception type of invalid insert operation");
[Test]
        public void Property_Code()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Style style = wb.CreateStyle();
            style.SetPatternColor(BackgroundType.Solid, Color.Red, Color.Green);
            cells[1048575, 0].SetStyle(style);
            Assert.AreEqual(BackgroundType.Solid, cells[1048575, 0].GetStyle().Pattern, "Before insert");
            cells.InsertRows(0, 2);
            Assert.AreEqual(BackgroundType.None, cells[1048575, 0].GetStyle().Pattern, "After insert");
            cells[1048575, 0].PutValue(1);
            bool fail = false;
            try
            {
                cells.InsertRows(0, 2);
                fail = true;
            }
            catch (CellsException e)
            {
                Assert.AreEqual(ExceptionType.Limitation, e.Code, "Exception type of invalid insert operation");
            }
            if (fail)
            {
                Assert.Fail("Insert operation should not be allowed when there are cells with data to be moved out of sheet");
            }
        }
```

### See Also

* enum [ExceptionType](../../exceptiontype/)
* class [CellsException](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


