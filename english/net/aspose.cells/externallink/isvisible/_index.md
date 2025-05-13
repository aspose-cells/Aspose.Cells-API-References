---
title: ExternalLink.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: ExternalLink property. Indicates whether this external link is visible in MS Excel
type: docs
url: /net/aspose.cells/externallink/isvisible/
---
## ExternalLink.IsVisible property

Indicates whether this external link is visible in MS Excel.

```csharp
public bool IsVisible { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets.ExternalLinks[1].IsVisible);
public void ExternalLink_Property_IsVisible()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Assert.AreEqual(2, workbook.Worksheets.ExternalLinks.Count);
    Assert.IsTrue(workbook.Worksheets.ExternalLinks[0].IsVisible);
    Assert.IsTrue(workbook.Worksheets.ExternalLinks[1].IsVisible);
    workbook = new Workbook(Constants.sourcePath + "example.xls");
    //if we parse macro , it's 2.but MS Excel only show one.
    Assert.AreEqual(2, workbook.Worksheets.ExternalLinks.Count);
    Assert.IsTrue(workbook.Worksheets.ExternalLinks[0].IsVisible);

}
```

### See Also

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


