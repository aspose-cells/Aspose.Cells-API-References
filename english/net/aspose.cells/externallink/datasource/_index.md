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
// Called: workbook.Worksheets.ExternalLinks[i].DataSource = NewLink;
[Test]
        public void Property_DataSource()
        {
            string NewLink;
            var searchString = "https://confidential.sharepoint.deshaw.com/managementreporting/";
            var replaceString = "https://deshaw0.sharepoint.com/sites/managementreporting/";
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet56760.xlsx");
            for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
            {
                NewLink = workbook.Worksheets.ExternalLinks[i].OriginalDataSource;
                NewLink = NewLink.Replace(searchString, replaceString);
                workbook.Worksheets.ExternalLinks[i].OriginalDataSource = NewLink;

                NewLink = workbook.Worksheets.ExternalLinks[i].DataSource;
                NewLink = NewLink.Replace(searchString, replaceString);
                workbook.Worksheets.ExternalLinks[i].DataSource = NewLink;
            }
            workbook.Save(Constants.destPath + "CellsNet56760.xlsx");
          string text=  ManualFileUtil.GetEntryText(Constants.destPath + "CellsNet56760.xlsx", "xl/metadata.xml");
            int p1 = text.IndexOf("<mdxMetadata");
            int p2 = text.IndexOf("<futureMetadata");
            Assert.IsTrue(p2 > p1);
        }
```

### See Also

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


