---
title: ExternalLink.OriginalDataSource
second_title: Aspose.Cells for .NET API Reference
description: ExternalLink property. Represents stored data source of the external link
type: docs
url: /net/aspose.cells/externallink/originaldatasource/
---
## ExternalLink.OriginalDataSource property

Represents stored data source of the external link.

```csharp
public string OriginalDataSource { get; set; }
```

### Examples

```csharp
// Called: string NewLink = workbook.Worksheets.ExternalLinks[i].OriginalDataSource;
public void ExternalLink_Property_OriginalDataSource()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
    {
        string NewLink = workbook.Worksheets.ExternalLinks[i].OriginalDataSource;
        NewLink = NewLink.Replace(@"https://arcusventures.sharepoint.com/Fund II/", @"/sites/shared/shared documents/Fund II/");
        workbook.Worksheets.ExternalLinks[i].OriginalDataSource = NewLink;
    }
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
    {
        string NewLink = workbook.Worksheets.ExternalLinks[i].OriginalDataSource;
      Assert.IsTrue(NewLink.IndexOf("/")!= -1);
    }
}
```

### See Also

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


