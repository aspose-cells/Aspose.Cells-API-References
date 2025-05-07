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
[Test]
        public void Method_RemoveUnusedStyles()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "xlsx/N52081.xlsx");
            wb.RemoveUnusedStyles();
            Util.ReSave(wb, SaveFormat.Xlsx);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


