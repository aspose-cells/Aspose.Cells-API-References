---
title: Cells.ConvertStringToNumericValue
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Converts all string data in the worksheet to numeric value if possible
type: docs
url: /net/aspose.cells/cells/convertstringtonumericvalue/
---
## Cells.ConvertStringToNumericValue method

Converts all string data in the worksheet to numeric value if possible.

```csharp
public void ConvertStringToNumericValue()
```

### Examples

```csharp
// Called: cells.ConvertStringToNumericValue();
[Test]
        public void Method_ConvertStringToNumericValue()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells["A1"];
            cell.PutValue("7/25/2016");

            cells.ConvertStringToNumericValue();
            Style style = cell.GetStyle();
            Assert.AreEqual("m/d/yyyy",style.Custom);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


