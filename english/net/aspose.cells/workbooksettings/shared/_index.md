---
title: WorkbookSettings.Shared
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets or sets a value that indicates whether the Workbook is shared
type: docs
url: /net/aspose.cells/workbooksettings/shared/
---
## WorkbookSettings.Shared property

Gets or sets a value that indicates whether the Workbook is shared.

```csharp
public bool Shared { get; set; }
```

### Remarks

The default value is false.

### Examples

```csharp
// Called: Assert.IsTrue(book.Settings.Shared);
[Test]
        public void Property_Shared()
        {
            var book = new Workbook();
            book.Settings.Shared = true;
            book.Save(Constants.destPath + &quot;CellsNet45517.xlsx&quot;);
            book = new Workbook(Constants.destPath + &quot;CellsNet45517.xlsx&quot;);
            Assert.IsTrue(book.Settings.Shared);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


