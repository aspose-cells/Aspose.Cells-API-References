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
// Called: saveOptions.ExportCellName = false;
public void Property_ExportCellName(string docFile, string newFile)
        {
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.ParsingFormulaOnOpen = true;

            FileStream fstream = new FileStream(docFile, FileMode.Open);
            Workbook workbook = new Workbook(fstream, loadOptions);
            workbook.FileFormat = FileFormatType.Xltm;
            fstream.Dispose();

            fstream = new FileStream(newFile, FileMode.Create);
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsm);
            saveOptions.ExportCellName = false;
            workbook.Save(fstream, saveOptions);
            fstream.Dispose();
        }
```

### See Also

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


