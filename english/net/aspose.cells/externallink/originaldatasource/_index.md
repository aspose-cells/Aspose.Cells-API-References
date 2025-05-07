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
// Called: Assert.AreEqual(book.Worksheets.ExternalLinks[0].OriginalDataSource, @"/_Work/Toronto/Parent/parent.xlsx");
[Test]
        public void Property_OriginalDataSource()
        {
            Workbook book = new Workbook(Constants.sourcePath + "CellsNet44402.xlsx");
            Assert.AreEqual(book.Worksheets.ExternalLinks[0].OriginalDataSource, @"/_Work/Toronto/Parent/parent.xlsx");
            Console.WriteLine(book.Worksheets.ExternalLinks[0].DataSource);
        }
```

### See Also

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


