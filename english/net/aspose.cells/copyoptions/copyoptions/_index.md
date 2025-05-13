---
title: CopyOptions.CopyOptions
second_title: Aspose.Cells for .NET API Reference
description: CopyOptions constructor. CopyOptions constructor
type: docs
url: /net/aspose.cells/copyoptions/copyoptions/
---
## CopyOptions constructor

CopyOptions constructor.

```csharp
public CopyOptions()
```

### Examples

```csharp
// Called: CopyOptions options = new CopyOptions();
public void CopyOptions_Constructor()
{
    var book = new Workbook(Constants.sourcePath + "example.xlsx");
    var source = book.Worksheets[0];
    var destination = book.Worksheets[book.Worksheets.Add()];
    CopyOptions options = new CopyOptions();
    options.ReferToDestinationSheet = true;

    destination.Cells.CopyRows(source.Cells, 0, 0, source.Cells.MaxDisplayRange.RowCount, options);
    Assert.AreEqual(destination.Charts[0].NSeries[0].Values, "=Sheet2!$B$2:$B$4");
    Util.ReSave(book, SaveFormat.Xlsx);
    //book.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


