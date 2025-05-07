---
title: Worksheet.IsRowColumnHeadersVisible
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true
type: docs
url: /net/aspose.cells/worksheet/isrowcolumnheadersvisible/
---
## Worksheet.IsRowColumnHeadersVisible property

Gets or sets a value indicating whether the worksheet will display row and column headers. Default is true.

```csharp
public bool IsRowColumnHeadersVisible { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].IsRowColumnHeadersVisible, false);
[Test, Category("Bug")]
        public void Property_IsRowColumnHeadersVisible()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].IsRowColumnHeadersVisible = false;
            workbook.Save(Constants.destPath + "Test_159075.xml");
            workbook = new Workbook(Constants.destPath + "Test_159075.xml");
            Assert.AreEqual(workbook.Worksheets[0].IsRowColumnHeadersVisible, false);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


