---
title: PaginatedSaveOptions.OnePagePerSheet
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. If OnePagePerSheet is true  all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid and the other settings of pagesetup will still take effect
type: docs
url: /net/aspose.cells/paginatedsaveoptions/onepagepersheet/
---
## PaginatedSaveOptions.OnePagePerSheet property

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Examples

```csharp
// Called: options.OnePagePerSheet = true;
public void PaginatedSaveOptions_Property_OnePagePerSheet()
{
    string path = Constants.TemplatePath + "NetCoreTests/CELLSNETCORE21/";
    string path2 = Constants.destPath + "NetCoreTests/";
    string excelPath = path + "example.xlsx";

    Workbook workbook = new Workbook(excelPath);
    PdfSaveOptions options = new PdfSaveOptions();
    options.OnePagePerSheet = true;
    workbook.Save(path2 + "win_out1.pdf", options);

}
```

### See Also

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


