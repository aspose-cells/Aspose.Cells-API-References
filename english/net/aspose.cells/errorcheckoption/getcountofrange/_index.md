---
title: ErrorCheckOption.GetCountOfRange
second_title: Aspose.Cells for .NET API Reference
description: ErrorCheckOption method. Gets the count of ranges that influenced by this setting
type: docs
url: /net/aspose.cells/errorcheckoption/getcountofrange/
---
## ErrorCheckOption.GetCountOfRange method

Gets the count of ranges that influenced by this setting.

```csharp
public int GetCountOfRange()
```

### Return Value

the count of ranges that influenced by this setting.

### Examples

```csharp
// Called: int c = workbook.Worksheets[0].ErrorCheckOptions[0].GetCountOfRange();
[Test]
        public void Method_GetCountOfRange()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET51050.xls&quot;);
            int c = workbook.Worksheets[0].ErrorCheckOptions[0].GetCountOfRange();
            workbook.Save(Constants.destPath + &quot;CELLSNET51050.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET51050.xls&quot;);
            Assert.AreEqual(c, workbook.Worksheets[0].ErrorCheckOptions[0].GetCountOfRange());
        }
```

### See Also

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


