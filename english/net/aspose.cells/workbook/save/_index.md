---
title: Workbook.Save
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Saves the workbook to the disk
type: docs
url: /net/aspose.cells/workbook/save/
---
## Save(string, SaveFormat) {#save_3}

Saves the workbook to the disk.

```csharp
public void Save(string fileName, SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The file name. |
| saveFormat | SaveFormat | The save format type. |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet and add some sample data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Save the workbook to XLSX format
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Save the workbook to PDF format
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### See Also

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string) {#save_2}

Save the workbook to the disk.

```csharp
public void Save(string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String |  |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add some sample data
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Save the workbook to different formats using string parameter
            workbook.Save("output.xlsx");
            workbook.Save("output.xls");
            workbook.Save("output.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string, SaveOptions) {#save_4}

Saves the workbook to the disk.

```csharp
public void Save(string fileName, SaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The file name. |
| saveOptions | SaveOptions | The save options. |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet and add some data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Create HTML save options and configure them
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportImagesAsBase64 = true;
            
            // Save the workbook with options
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("Workbook saved successfully with HTML options.");
        }
    }
}
```

### See Also

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveFormat) {#save}

Saves the workbook to the stream.

```csharp
public void Save(Stream stream, SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The file stream. |
| saveFormat | SaveFormat | The save file format type. |

### Examples

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStreamSaveFormatDemo
    {
        public static void Run()
        {
            // Create a sample workbook
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test Save with Stream");
            
            // Save to memory stream in MHTML format
            using (MemoryStream stream = new MemoryStream())
            {
                wb.Save(stream, SaveFormat.MHtml);
                
                // Reset stream position and save to file
                stream.Seek(0, SeekOrigin.Begin);
                string outputPath = "output.mht";
                using (StreamReader sr = new StreamReader(stream))
                using (StreamWriter sw = new StreamWriter(outputPath, false, Encoding.UTF8))
                {
                    sw.Write(sr.ReadToEnd());
                }
            }
        }
    }
}
```

### See Also

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveOptions) {#save_1}

Saves the workbook to the stream.

```csharp
public void Save(Stream stream, SaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The file stream. |
| saveOptions | SaveOptions | The save options. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSaveWithStreamSaveOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add some data to the worksheet
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Prepare SaveOptions
            var saveOptions = new XlsbSaveOptions();
            
            // Create a memory stream to save the workbook
            using (MemoryStream stream = new MemoryStream())
            {
                try
                {
                    // Call the Save method with Stream and SaveOptions parameters
                    workbook.Save(stream, saveOptions);
                    
                    Console.WriteLine("Workbook saved successfully to stream with XLSB format");
                    
                    // Demonstrate the effect by checking stream length
                    Console.WriteLine($"Stream length after save: {stream.Length} bytes");
                    
                    // Optional: Save the stream to a file for verification
                    File.WriteAllBytes("WorkbookSaveWithStreamSaveOptions.xlsb", stream.ToArray());
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error saving workbook: {ex.Message}");
                }
            }
        }
    }
}
```

### See Also

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions) {#save_5}

Creates the result spreadsheet and transfer it to the client then open it in the browser or MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| response | HttpResponse | Response object to return the spreadsheet to client. |
| fileName | String | The name of created file. |
| contentDisposition | ContentDisposition | The content disposition type. |
| saveOptions | SaveOptions | The save options. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Net.Mime;
    using Aspose.Cells.Rendering;

    public class WorkbookMethodSaveWithHttpResponseStringContentDispoDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add some sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            try
            {
                // Create a mock response stream (in a real application, this would be the actual response)
                using (var memoryStream = new System.IO.MemoryStream())
                {
                    // Prepare parameters for Save method
                    string fileName = "output.xlsx";
                    ContentDisposition contentDisposition = new ContentDisposition
                    {
                        DispositionType = DispositionTypeNames.Attachment,
                        FileName = fileName
                    };
                    SaveOptions saveOptions = new XlsSaveOptions(SaveFormat.Xlsx);
                    
                    // Save to stream instead of HttpResponse
                    workbook.Save(memoryStream, saveOptions);
                    
                    Console.WriteLine("Workbook saved successfully (simulated HttpResponse)");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions, bool) {#save_6}

Creates the result spreadsheet and transfer it to the client then open it in the browser or MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions, bool enableHttpCompression)
```

| Parameter | Type | Description |
| --- | --- | --- |
| response | HttpResponse | Response object to return the spreadsheet to client. |
| fileName | String | The name of created file. |
| contentDisposition | ContentDisposition | The content disposition type. |
| saveOptions | SaveOptions | The save options. |
| enableHttpCompression | Boolean | whether http compression is to be used |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;
    using System.Net.Mime;

    public class WorkbookMethodSaveWithHttpResponseStringContentDispoDemo1
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue(123.45);
            
            try
            {
                // Create a mock HttpResponse (in real scenario this would come from web context)
                // Using MemoryStream instead of HttpResponse since we don't have System.Web reference
                using (MemoryStream stream = new MemoryStream())
                {
                    // Prepare parameters for Save method
                    string fileName = "WorkbookOutput.xlsx";
                    ContentDisposition contentDisposition = new ContentDisposition
                    {
                        DispositionType = DispositionTypeNames.Attachment,
                        FileName = fileName
                    };
                    SaveOptions saveOptions = new XlsSaveOptions(SaveFormat.Xlsx);
                    bool clearData = true;
                    
                    // Call the Save method with stream instead of HttpResponse
                    workbook.Save(stream, saveOptions);
                    
                    Console.WriteLine("Workbook saved to stream successfully");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
            
            // Save locally as well to demonstrate the effect
            workbook.Save("LocalSaveDemo.xlsx");
        }
    }
}
```

### See Also

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


