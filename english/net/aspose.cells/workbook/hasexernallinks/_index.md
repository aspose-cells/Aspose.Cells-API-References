---
title: Workbook.HasExernalLinks
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Indicates whether this workbook contains external links to other data sources
type: docs
url: /net/aspose.cells/workbook/hasexernallinks/
---
## Workbook.HasExernalLinks method

Indicates whether this workbook contains external links to other data sources.

```csharp
[Obsolete("Use ExternalLinkCollection.Count property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasExernalLinks()
```

### Return Value

Whether this workbook contains external links to other data sources.

### Remarks

NOTE: This member is now obsolete. Instead, please use ExternalLinkCollection.Count to check whether there are external links in this workbook. This method will be removed 12 months later since December 2021. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: if (workbook.HasExernalLinks()) //Process those with external links
public void Workbook_Method_HasExernalLinks()
{
    var workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xlsx");
    if (workbook.HasExernalLinks()) //Process those with external links 
    {

        var links = workbook.Worksheets.ExternalLinks;

        Assert.IsFalse(links[0].IsVisible);
        Assert.IsTrue(links[4].IsVisible);
    }
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


