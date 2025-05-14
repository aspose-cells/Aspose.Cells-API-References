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
public void DeleteOptions_Property_UpdateReference()
{
    Workbook workbook  =new Workbook(Constants.sourcePath + "example.xlsm");
    DeleteOptions deleteOptions = new DeleteOptions();
    deleteOptions.UpdateReference = true;

    workbook.Worksheets[0].Cells.DeleteBlankColumns(deleteOptions);
    workbook.Save(Constants.destPath + "example.xlsm");
}
```

### See Also

* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


