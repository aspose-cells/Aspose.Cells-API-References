---
title: Cell.Type
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Represents cell value type
type: docs
url: /net/aspose.cells/cell/type/
---
## Cell.Type property

Represents cell value type.

```csharp
public CellValueType Type { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(CellValueType.IsNumeric, cell.Type);
[Test]
        public void Property_Type()
        {
            Workbook wb = new Workbook();
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();
            style.Number = 14;
            cell.SetStyle(style);
            cell.PutValue(8995080);
            Assert.AreEqual(CellValueType.IsNumeric, cell.Type);
            string res = cell.StringValue;
            if (res.Length < 10 || res.Replace("#", "").Length > 0)
            {
                Assert.Fail("Invalid datetime should not be formatted as " + res);
            }
            cell.PutValue(-899508);
            Assert.AreEqual(CellValueType.IsNumeric, cell.Type);
            res = cell.StringValue;
            if (res.Length < 10 || res.Replace("#", "").Length > 0)
            {
                Assert.Fail("Invalid datetime should not be formatted as " + res);
            }
        }
```

### See Also

* enum [CellValueType](../../cellvaluetype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


