---
title: DeleteBlankOptions.DrawingsAsBlank
second_title: Aspose.Cells for .NET API Reference
description: DeleteBlankOptions property. Whether drawing related objects such as picture shape chart... will be taken as blank. Default value is true
type: docs
url: /net/aspose.cells/deleteblankoptions/drawingsasblank/
---
## DeleteBlankOptions.DrawingsAsBlank property

Whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true.

```csharp
public bool DrawingsAsBlank { get; set; }
```

### Remarks

When setting this property as false, all rows/columns covered by drawing objects will not be taken as blank and will not be deleted.

### Examples

```csharp
// Called: options.DrawingsAsBlank = false;
[Test]
        public void Property_DrawingsAsBlank()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET45393.xls&quot;);
            DeleteBlankOptions options = new DeleteBlankOptions();
            options.UpdateReference = true;
            options.DrawingsAsBlank = false;

            foreach (Worksheet sheet in workbook.Worksheets)
            {
                sheet.Cells.DeleteBlankColumns(options);
                sheet.Cells.DeleteBlankRows(options);
            }
            Assert.AreEqual(1, workbook.Worksheets[0].Shapes.Count);
            Assert.IsTrue(workbook.Worksheets[0].Shapes[0].Width &gt; 0);
            Assert.IsTrue(workbook.Worksheets[0].Shapes[0].Height &gt; 0);
        }
```

### See Also

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


