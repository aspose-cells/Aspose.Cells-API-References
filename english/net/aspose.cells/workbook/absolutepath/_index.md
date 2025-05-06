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
[Test]
        public void Property_AbsolutePath()
        {
            Workbook sourceBook = new Workbook(Constants.sourcePath + &quot;CELLSNETCORE65.xlsx&quot;);
            string pathToBook = Path.Combine(sourceBook.AbsolutePath, sourceBook.FileName);
            SetHyperlink(sourceBook.Worksheets[1], 0, pathToBook, sourceBook.Worksheets[1].Name, &quot;A1&quot;);
            SetHyperlink(sourceBook.Worksheets[1], 1, pathToBook, sourceBook.Worksheets[2].Name, &quot;A1&quot;);

            sourceBook.Save(Constants.destPath + &quot;dest.xlsx&quot;);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


