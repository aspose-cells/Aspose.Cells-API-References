---
title: Validation.GetValue
second_title: Aspose.Cells for .NET API Reference
description: Validation method. Get the value of validation on the specific cell
type: docs
url: /net/aspose.cells/validation/getvalue/
---
## Validation.GetValue method

Get the value of validation on the specific cell.

```csharp
public object GetValue(int row, int column, bool isValue1)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
| isValue1 | Boolean | Indicates whether getting the first value. |

### Examples

```csharp
// Called: object val = dv.GetValue(1, 1, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET53977.xlsx&quot;);
            Validation dv = wb.Worksheets[0].Cells[&quot;B2&quot;].GetValidation();
            object val = dv.GetValue(1, 1, true);
            object[] objects = val as object[];
            Assert.AreEqual(&quot;Attachment Included&quot;, objects[0]);


            wb.Save(Constants.destPath + &quot;CELLSNET53977.xlsx&quot;);
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


