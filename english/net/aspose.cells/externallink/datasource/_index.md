---
title: ExternalLink.DataSource
second_title: Aspose.Cells for .NET API Reference
description: ExternalLink property. Represents data source of the external link
type: docs
url: /net/aspose.cells/externallink/datasource/
---
## ExternalLink.DataSource property

Represents data source of the external link.

```csharp
public string DataSource { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(workbook.Worksheets.ExternalLinks[1].DataSource.StartsWith(@"\\DEMO50\FileShare"));
public void ExternalLink_Property_DataSource()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.IsFalse(workbook.Worksheets.ExternalLinks[1].DataSource.StartsWith(@"\\DEMO50\FileShare"));
}
```

### See Also

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


