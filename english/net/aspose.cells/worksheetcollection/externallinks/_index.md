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
// Called: workbook.Worksheets.ExternalLinks[0].DataSource = workbook2;
public void WorksheetCollection_Property_ExternalLinks()
{
            
    const string workbook2 = "example.xlsx";

    var workbook = new Workbook(Constants.sourcePath  + "example.xlsx");
    //CELLSNET-55418
   // Assert.AreEqual("http://schemas.openxmlformats.org/officeDocument/2006/relationships/externalLinkPath", workbook.Worksheets.ExternalLinks[0].PathType);
    Assert.AreEqual("example.xlsx", workbook.Worksheets.ExternalLinks[0].DataSource);
    Console.WriteLine();

    workbook.Worksheets.ExternalLinks[0].DataSource = workbook2;
    Console.WriteLine("External list data source is updated to {0}", workbook2);
    Console.WriteLine("External list data source = {0}", workbook.Worksheets.ExternalLinks[0].DataSource);
    Console.WriteLine();

    workbook.Save(Constants.destPath + "example.xlsx");
    Console.WriteLine("Workbook is saved.");
    Console.WriteLine();

    workbook.Dispose();
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual("example.xlsx", workbook.Worksheets.ExternalLinks[0].OriginalDataSource);
}
```

### See Also

* class [ExternalLinkCollection](../../externallinkcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


