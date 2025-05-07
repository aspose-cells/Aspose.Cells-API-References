---
title: WorksheetCollection.ExternalLinks
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Represents external links in a workbook
type: docs
url: /net/aspose.cells/worksheetcollection/externallinks/
---
## WorksheetCollection.ExternalLinks property

Represents external links in a workbook.

```csharp
public ExternalLinkCollection ExternalLinks { get; }
```

### Examples

```csharp
// Called: references = workbook.Worksheets.ExternalLinks;
[Test]
        // http://www.aspose.com/community/forums/thread/239318.aspx
        public void Property_ExternalLinks()
        {
            Console.WriteLine("Property_ExternalLinks()");
            string infn = path + "Test_WorksheetsExternalLinksAttr.xlsx";
            string outfn = Constants.destPath + "Test_WorksheetsExternalLinksAttr_out.xlsx";

            Workbook workbook = new Workbook();
            ExternalLinkCollection references = workbook.Worksheets.ExternalLinks;
            Console.WriteLine("Worksheets.ExternalLinks.Count before open:" + references.Count);
            workbook = new Workbook(infn);
            references = workbook.Worksheets.ExternalLinks;
            Console.WriteLine("Worksheets.ExternalLinks.Count after open:" + references.Count);
            workbook.Save(outfn);
        }
```

### See Also

* class [ExternalLinkCollection](../../externallinkcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


