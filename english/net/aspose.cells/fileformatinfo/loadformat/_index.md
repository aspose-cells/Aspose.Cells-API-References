---
title: FileFormatInfo.LoadFormat
second_title: Aspose.Cells for .NET API Reference
description: FileFormatInfo property. Gets the detected load format
type: docs
url: /net/aspose.cells/fileformatinfo/loadformat/
---
## FileFormatInfo.LoadFormat property

Gets the detected load format.

```csharp
public LoadFormat LoadFormat { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(o.LoadFormat.ToString());
public void FileFormatInfo_Property_LoadFormat()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET45478/";

    string fileName = "SAMPLE_XLS_ISSUE.XLS";
    //Your excel file is actually an HTML file. 
    var o = FileFormatUtil.DetectFileFormat(filePath + fileName);
    Console.WriteLine(o.LoadFormat.ToString());
    //Now load your file with correct format 
    LoadOptions ldps = new LoadOptions(LoadFormat.MHtml);
    var workbook = new Workbook(filePath + "SAMPLE_XLS_ISSUE.XLS", ldps);
    workbook.Worksheets[0].AutoFitColumns();
    workbook.Save(CreateFolder(filePath) + "out_issue.xlsx");

    //fileName = "Sample_file_open_error.xls";
    //workbook = new Workbook(CreateFolder(filePath) + fileName, ldps);
    //workbook.Worksheets[0].AutoFitColumns();
    //workbook.Save(CreateFolder(filePath) + "out_error.xlsx");

}
```

### See Also

* enum [LoadFormat](../../loadformat/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


