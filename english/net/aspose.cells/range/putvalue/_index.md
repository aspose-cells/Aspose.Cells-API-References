---
title: Range.PutValue
second_title: Aspose.Cells for .NET API Reference
description: Range method. Puts a value into the range if appropriate the value will be converted to other data type and cells number format will be reset
type: docs
url: /net/aspose.cells/range/putvalue/
---
## Range.PutValue method

Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
| isConverted | Boolean | True: converted to other data type if appropriate. |
| setStyle | Boolean | True: set the number format to cell's style when converting to other data type |

### Examples

```csharp
// Called: range.PutValue("123", true, false);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1:B10");
            range.PutValue("123", true, false);
            Assert.AreEqual(cells["A5"].DoubleValue, 123);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


