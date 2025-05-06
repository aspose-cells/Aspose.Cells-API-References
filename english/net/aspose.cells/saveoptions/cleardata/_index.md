---
title: SaveOptions.ClearData
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. Make the workbook empty after saving the file
type: docs
url: /net/aspose.cells/saveoptions/cleardata/
---
## SaveOptions.ClearData property

Make the workbook empty after saving the file.

```csharp
public bool ClearData { get; set; }
```

### Examples

```csharp
// Called: pdfSaveOptions.ClearData = true;
[Test]
        public void Property_ClearData()
        {
            string FileName = Constants.sourcePath + &quot;TestWorkbook\\Book2.xls&quot;;
            Workbook workbook = new Workbook(FileName);
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.ClearData = true;
            workbook.Save(Constants.destPath + &quot;testSave.pdf&quot;, pdfSaveOptions);
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


