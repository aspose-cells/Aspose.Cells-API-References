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
// Called: ws.Cells.DeleteBlankColumns(new DeleteBlankOptions() { DrawingsAsBlank = false });
[Test]
        public void Property_DrawingsAsBlank()
        {  
            Workbook wb = new Workbook(Constants.sourcePath +"CELLSNET-45428.xlsx");
            foreach (Worksheet ws in wb.Worksheets)
            {
                ws.Cells.DeleteBlankRows();
                ws.Cells.DeleteBlankColumns(new DeleteBlankOptions() { DrawingsAsBlank = false });
            }
            Assert.AreEqual(1, wb.Worksheets[0].Charts.Count);
            //wb.Save(Constants.destPath + "CELLSNET45428.xlsx");
            Util.ReSave(wb, SaveFormat.Xlsx);
        }
```

### See Also

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


