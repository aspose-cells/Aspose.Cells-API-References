---
title: Hyperlink.Delete
second_title: Aspose.Cells for .NET API Reference
description: Hyperlink method. Deletes this hyperlink
type: docs
url: /net/aspose.cells/hyperlink/delete/
---
## Hyperlink.Delete method

Deletes this hyperlink

```csharp
public void Delete()
```

### Examples

```csharp
// Called: currentHyperlink.Delete(); // error here
public void Hyperlink_Method_Delete()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlt");

    foreach (Worksheet worksheet in workbook.Worksheets)
    {
        for (int i = worksheet.Hyperlinks.Count - 1; i >= 0; i--)
        {
            var currentHyperlink = worksheet.Hyperlinks[i];
            currentHyperlink.Delete(); // error here
        }
    }
}
```

### See Also

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


