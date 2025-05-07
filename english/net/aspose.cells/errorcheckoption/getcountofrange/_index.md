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
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET51050.xls");
            int c = workbook.Worksheets[0].ErrorCheckOptions[0].GetCountOfRange();
            workbook.Save(Constants.destPath + "CELLSNET51050.xls");
            workbook = new Workbook(Constants.destPath + "CELLSNET51050.xls");
            Assert.AreEqual(c, workbook.Worksheets[0].ErrorCheckOptions[0].GetCountOfRange());
        }
```

### See Also

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


