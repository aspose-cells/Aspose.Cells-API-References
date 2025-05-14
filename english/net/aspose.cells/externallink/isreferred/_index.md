---
title: ExternalLink.IsReferred
second_title: Aspose.Cells for .NET API Reference
description: ExternalLink property. Indicates whether this external link is referenced by others
type: docs
url: /net/aspose.cells/externallink/isreferred/
---
## ExternalLink.IsReferred property

Indicates whether this external link is referenced by others.

```csharp
public bool IsReferred { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets.ExternalLinks[0].IsReferred);
public void ExternalLink_Property_IsReferred()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.IsTrue(workbook.Worksheets.ExternalLinks[0].IsReferred);
}
```

### See Also

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


