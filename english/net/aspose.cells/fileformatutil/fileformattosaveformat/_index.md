---
title: FileFormatUtil.FileFormatToSaveFormat
second_title: Aspose.Cells for .NET API Reference
description: FileFormatUtil method. Converting file format to save format
type: docs
url: /net/aspose.cells/fileformatutil/fileformattosaveformat/
---
## FileFormatUtil.FileFormatToSaveFormat method

Converting file format to save format.

```csharp
public static SaveFormat FileFormatToSaveFormat(FileFormatType format)
```

| Parameter | Type | Description |
| --- | --- | --- |
| format | FileFormatType | The file format type. |

### Examples

```csharp
// Called: Util.ReSave(excel, FileFormatUtil.FileFormatToSaveFormat(excel.FileFormat));
public void FileFormatUtil_Method_FileFormatToSaveFormat()
{
    //Test1_U227969_TestAsposeMassivReadWrite1.xlsx
    string[] files = Directory.GetFiles(Constants.sourcePath + "openxls/");

    Workbook excel = new Workbook();
    string fileName = "";
    foreach (string file in files)
    {
        try
        {
            excel = new Workbook(file);
            int index = file.LastIndexOf("/");
            fileName = file.Substring(index);

            Util.ReSave(excel, FileFormatUtil.FileFormatToSaveFormat(excel.FileFormat));
        }
        catch (Exception e)
        {
            Console.WriteLine("Problem in processing " + file);
            Console.WriteLine("    " + e.GetType().Name + ": " + e.Message);
        }
    }
}
```

### See Also

* enum [SaveFormat](../../saveformat/)
* enum [FileFormatType](../../fileformattype/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


