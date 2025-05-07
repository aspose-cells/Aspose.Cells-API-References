---
title: Worksheet.Split
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Splits window
type: docs
url: /net/aspose.cells/worksheet/split/
---
## Worksheet.Split method

Splits window.

```csharp
public void Split()
```

### Examples

```csharp
// Called: workbook.Worksheets[0].Split();
[Test, Category("Bug")]
        public void Method_Split()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Split();
            workbook.Save(Constants.destPath + "TestSpilt_001.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "TestSpilt_001.xml");
            // Assert.AreEqual(workbook.Worksheets[0].pa
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


