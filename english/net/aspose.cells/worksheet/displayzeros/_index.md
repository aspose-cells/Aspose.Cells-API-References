---
title: Worksheet.DisplayZeros
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. True if zero values are displayed
type: docs
url: /net/aspose.cells/worksheet/displayzeros/
---
## Worksheet.DisplayZeros property

True if zero values are displayed.

```csharp
public bool DisplayZeros { get; set; }
```

### Examples

```csharp
// Called: workbook.Worksheets[0].DisplayZeros = false;
[Test]
        public void Property_DisplayZeros()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].DisplayZeros = false;
            workbook.Save(Constants.destPath + "Test_163547.xls");
            workbook = new Workbook(Constants.destPath + "Test_163547.xls");
            Assert.AreEqual(workbook.Worksheets[0].DisplayZeros, false);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


