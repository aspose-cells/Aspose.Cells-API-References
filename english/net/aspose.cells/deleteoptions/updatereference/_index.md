---
title: DeleteOptions.UpdateReference
second_title: Aspose.Cells for .NET API Reference
description: DeleteOptions property. Indicates if update references in other worksheets
type: docs
url: /net/aspose.cells/deleteoptions/updatereference/
---
## DeleteOptions.UpdateReference property

Indicates if update references in other worksheets.

```csharp
public bool UpdateReference { get; set; }
```

### Examples

```csharp
// Called: deleteOptions.UpdateReference = true;
[Test]
        public void Property_UpdateReference()
        {
            DeleteOptions deleteOptions = new DeleteOptions();
            deleteOptions.UpdateReference = true;
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsCore89.xlsx&quot;);
            wb.Worksheets[0].Cells.DeleteBlankColumns(deleteOptions);
            wb.Worksheets[0].Cells.DeleteBlankRows(deleteOptions);
            wb.Save(Constants.destPath + &quot;CellsCore89.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CellsCore89.xlsx&quot;);
            wb.Save(Constants.destPath + &quot;CellsCore89.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CellsCore89.xlsx&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;C1&quot;].Comment.ThreadedComments.Count, 1);
        }
```

### See Also

* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


