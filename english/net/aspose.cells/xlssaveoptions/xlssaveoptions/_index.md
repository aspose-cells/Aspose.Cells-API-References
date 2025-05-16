---
title: XlsSaveOptions.XlsSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: XlsSaveOptions constructor. Creates options for saving Excel 972003 xls file
type: docs
url: /net/aspose.cells/xlssaveoptions/xlssaveoptions/
---
## XlsSaveOptions() {#constructor}

Creates options for saving Excel 97-2003 xls file.

```csharp
public XlsSaveOptions()
```

### Examples

```csharp
// Called: XlsSaveOptions saveOptions = new XlsSaveOptions();
public void XlsSaveOptions_Constructor()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47308/";

    Workbook wb = new Workbook();
    Worksheet ws = wb.Worksheets[0];
    string htmlString1 = "<font style=\"font-weight:normal; text-decoration:underline;color:red;\">Red1</font><font style=\"font-weight:normal;text-decoration:underline;color:green;\">Green1</font>";
    var cell1 = ws.Cells[1, 1];
    cell1.HtmlString = htmlString1;

    //string htmlString2 = "<font style=\"font-weight:normal; text-decoration:underline;color:red;\">Red2</font><font style=\"font-weight:normal;text-decoration:underline;color:green;\">Green2</font>";
    var cell2 = ws.Cells[3, 1];
    cell2.HtmlString = htmlString1;
    var range2 = ws.Cells.CreateRange(3, 1, 5, 5);
    range2.Merge();
    XlsSaveOptions saveOptions = new XlsSaveOptions();

    string savePath = CreateFolder(filePath);
    wb.Save(savePath + @"out.xls", saveOptions);

    HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
    wb.Save(savePath + @"out.htm", htmlSaveOptions);
}
```

### See Also

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XlsSaveOptions(SaveFormat) {#constructor_1}

Creates options for saving Excel 97-2003 xls/xlt file.

```csharp
public XlsSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be Excel97To2003 or Xlt, otherwise the saved format will be set as Excel97To2003 automatically. |

### Examples

```csharp
namespace AsposeCellsExamples.XlsSaveOptionsMethodCtorWithSaveFormatDemo
{
    using Aspose.Cells;
    using System;

    public class XlsSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add some sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue(123.45);
            
            try
            {
                // Call the #ctor method with SaveFormat parameter
                XlsSaveOptions saveOptions = new XlsSaveOptions(SaveFormat.Excel97To2003);
                
                // Set additional properties
                saveOptions.MatchColor = true;
                saveOptions.WpsCompatibility = false;
                
                Console.WriteLine("XlsSaveOptions constructor executed successfully with SaveFormat parameter");
                
                // Save the workbook with the specified options
                workbook.Save("XlsSaveOptionsCtorDemo.xls", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XlsSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [SaveFormat](../../saveformat/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


