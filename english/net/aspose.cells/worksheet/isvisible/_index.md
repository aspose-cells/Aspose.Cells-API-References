---
title: Worksheet.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents if the worksheet is visible
type: docs
url: /net/aspose.cells/worksheet/isvisible/
---
## Worksheet.IsVisible property

Represents if the worksheet is visible.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(workbook.Worksheets[1].IsVisible);
[Test]
        public void Property_IsVisible()
        {
            JAVA41173();
            Workbook workbook = new Workbook(_destFilesPath + "JAVA41173.html");
            Assert.AreEqual(4, workbook.Worksheets.Count);
            Assert.IsFalse(workbook.Worksheets[1].IsVisible);

        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


