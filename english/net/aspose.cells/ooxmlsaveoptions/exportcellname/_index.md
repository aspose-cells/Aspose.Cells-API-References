---
title: OoxmlSaveOptions.ExportCellName
second_title: Aspose.Cells for .NET API Reference
description: OoxmlSaveOptions property. Indicates if export cell name to Excel2007 .xlsx .xlsm .xltx .xltm file. If the output file may be accessed by SQL Server DTS this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true
type: docs
url: /net/aspose.cells/ooxmlsaveoptions/exportcellname/
---
## OoxmlSaveOptions.ExportCellName property

Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true.

```csharp
public bool ExportCellName { get; set; }
```

### Examples

```csharp
// Called: xlsxSaveOptions.ExportCellName = true;
public void OoxmlSaveOptions_Property_ExportCellName()
{
    Console.WriteLine("testCELLSNET_27446()");
    string infn = path + @"example.xlsx";
    string outfn = destpath + @"example.xlsm";
    string outfn1 = destpath + @"example.xlsx";

    Workbook wb = new Workbook(infn);
    OoxmlSaveOptions xlsxSaveOptions = new OoxmlSaveOptions(SaveFormat.Xlsm);
    xlsxSaveOptions.ExportCellName = true;
    wb.Save(outfn, xlsxSaveOptions);
    xlsxSaveOptions = new OoxmlSaveOptions();
    xlsxSaveOptions.ExportCellName = true;
    wb.Save(outfn1, xlsxSaveOptions);


}
```

### See Also

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


