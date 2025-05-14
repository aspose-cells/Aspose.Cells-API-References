---
title: Workbook.RemoveUnusedStyles
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Remove all unused styles
type: docs
url: /net/aspose.cells/workbook/removeunusedstyles/
---
## Workbook.RemoveUnusedStyles method

Remove all unused styles.

```csharp
public void RemoveUnusedStyles()
```

### Examples

```csharp
// Called: wb.RemoveUnusedStyles();
public void Workbook_Method_RemoveUnusedStyles()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    PdfSaveOptions saveOpts = new PdfSaveOptions();
    wb.RemoveUnusedStyles();
    wb.Save(Constants.destPath + "example.pdf"); 
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


