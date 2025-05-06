---
title: Worksheet.IsProtected
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates if the worksheet is protected
type: docs
url: /net/aspose.cells/worksheet/isprotected/
---
## Worksheet.IsProtected property

Indicates if the worksheet is protected.

```csharp
public bool IsProtected { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(workbook.Worksheets[0].IsProtected);
[Test]
        public void Property_IsProtected()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET45739.xml&quot;);
            Assert.IsFalse(workbook.Worksheets[0].IsProtected);
            workbook.Save(Constants.destPath + &quot;CELLSNET45739.xml&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET45739.xml&quot;);
            Assert.IsFalse(workbook.Worksheets[0].IsProtected);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


