---
title: PaginatedSaveOptions.DefaultFont
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. When characters in the Excel are Unicode and not be set with correct font in cell style They may appear as block in pdfimage. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set Aspose.Cells will use system default font to show these unicode characters
type: docs
url: /net/aspose.cells/paginatedsaveoptions/defaultfont/
---
## PaginatedSaveOptions.DefaultFont property

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

```csharp
public string DefaultFont { get; set; }
```

### Examples

```csharp
// Called: pdfSaveOptions.DefaultFont = &amp;quot;Verdana&amp;quot;;
[Ignore(&quot;PdfSaveOptions.DefaultFont need fixed&quot;)]
        public void Property_DefaultFont()
        {
            string FileName = Constants.sourcePath + &quot;TestWorkbook\\Book2.xls&quot;;
            Workbook workbook = new Workbook(FileName);
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.DefaultFont = &quot;Verdana&quot;;            
            workbook.Save(Constants.destPath + &quot;testSave.pdf&quot;, pdfSaveOptions);
        }
```

### See Also

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


