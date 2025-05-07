---
title: ExternalLinkCollection.Count
second_title: Aspose.Cells for .NET API Reference
description: ExternalLinkCollection property. Gets the number of elements actually contained in the collection
type: docs
url: /net/aspose.cells/externallinkcollection/count/
---
## ExternalLinkCollection.Count property

Gets the number of elements actually contained in the collection.

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
[Test]
        public void Property_Count()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet46042.xlsx");
            for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
            {
                string NewLink = workbook.Worksheets.ExternalLinks[i].OriginalDataSource;
                NewLink = NewLink.Replace(@"https://arcusventures.sharepoint.com/Fund II/", @"/sites/shared/shared documents/Fund II/");
                workbook.Worksheets.ExternalLinks[i].OriginalDataSource = NewLink;
            }
            workbook.Save(Constants.destPath + "CellsNet46042.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet46042.xlsx");
            for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
            {
                string NewLink = workbook.Worksheets.ExternalLinks[i].OriginalDataSource;
              Assert.IsTrue(NewLink.IndexOf("/")!= -1);
            }
        }
```

### See Also

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


