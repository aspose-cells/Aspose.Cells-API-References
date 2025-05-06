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
// Called: Assert.IsFalse(workbook.Worksheets[0].DisplayZeros);
[Test, Category(&quot;Bug&quot;)]
        public void Property_DisplayZeros()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].DisplayZeros = false;
            workbook.Save(Constants.destPath + &quot;Test_209640.xml&quot;);
            workbook = new Workbook(Constants.destPath + &quot;Test_209640.xml&quot;);
            Assert.IsFalse(workbook.Worksheets[0].DisplayZeros);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


