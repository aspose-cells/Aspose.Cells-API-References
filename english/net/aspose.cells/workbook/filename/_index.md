---
title: Workbook.FileName
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets and sets the current file name
type: docs
url: /net/aspose.cells/workbook/filename/
---
## Workbook.FileName property

Gets and sets the current file name.

```csharp
public string FileName { get; set; }
```

### Remarks

If the file is opened by stream and there are some external formula references, please set the file name.

### Examples

```csharp
// Called: string pathToBook = Path.Combine(sourceBook.AbsolutePath, sourceBook.FileName);
[Test]
        public void Property_FileName()
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


