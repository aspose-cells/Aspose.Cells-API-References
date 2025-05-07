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
// Called: var deleteOptions = new DeleteOptions { UpdateReference = true };
[Test]
        public void Property_UpdateReference()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSNET46792.xlsx");
            var deleteOptions = new DeleteOptions { UpdateReference = true };
            foreach (Worksheet sheet in wb.Worksheets)
            {
                sheet.Cells.DeleteBlankRows(deleteOptions);
                sheet.Cells.DeleteBlankColumns(deleteOptions);
                sheet.AutoFitRows(true);
            }
            Util.ReSave(wb, SaveFormat.Xlsx);
            //bad case without assertion
            //wb.Save(Constants.destPath + "CELLSNET46792.xlsx");
        }
```

### See Also

* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


