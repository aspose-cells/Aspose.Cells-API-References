---
title: Workbook.AbsolutePath
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets and sets the absolute path of the file
type: docs
url: /net/aspose.cells/workbook/absolutepath/
---
## Workbook.AbsolutePath property

Gets and sets the absolute path of the file.

```csharp
public string AbsolutePath { get; set; }
```

### Remarks

Only used for external links.

### Examples

```csharp
// Called: string pathToBook = Path.Combine(sourceBook.AbsolutePath, sourceBook.FileName);
public void Workbook_Property_AbsolutePath()
{
    Workbook sourceBook = new Workbook(Constants.sourcePath + "example.xlsx");
    string pathToBook = Path.Combine(sourceBook.AbsolutePath, sourceBook.FileName);
    SetHyperlink(sourceBook.Worksheets[1], 0, pathToBook, sourceBook.Worksheets[1].Name, "A1");
    SetHyperlink(sourceBook.Worksheets[1], 1, pathToBook, sourceBook.Worksheets[2].Name, "A1");

    sourceBook.Save(Constants.destPath + "dest.xlsx");
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


