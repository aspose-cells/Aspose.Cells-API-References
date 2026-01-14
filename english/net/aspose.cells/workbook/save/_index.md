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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSaveWithStreamSaveFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet and add some sample data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            try
            {
                // Create a memory stream to save the workbook
                using (MemoryStream stream = new MemoryStream())
                {
                    // Save the workbook to the stream in XLSX format
                    workbook.Save(stream, SaveFormat.Xlsx);

                    // Display success message
                    Console.WriteLine("Workbook saved to stream successfully in XLSX format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // Reset stream position for potential further processing
                    stream.Position = 0;

                    // Optionally save to file for verification
                    using (FileStream fileStream = File.Create("StreamSaveDemo.xlsx"))
                    {
                        stream.CopyTo(fileStream);
                    }
                    Console.WriteLine("Stream content also saved to file: StreamSaveDemo.xlsx");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook to stream: {ex.Message}");
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

            // Access the first worksheet and add some data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Hello, Aspose.Cells!";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            // Create a MemoryStream to save the workbook
            MemoryStream stream = new MemoryStream();

            try
            {
                // Create SaveOptions for PDF format
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Save the workbook to the stream with the specified options
                workbook.Save(stream, saveOptions);

                Console.WriteLine("Workbook saved to stream successfully in PDF format.");
                Console.WriteLine($"Stream length: {stream.Length} bytes");

                // Reset stream position for potential further use
                stream.Position = 0;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
            finally
            {
                // Clean up resources
                stream?.Dispose();
                workbook?.Dispose();
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

### Remarks

This method is avaiable for net4.x versions only.

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

### Remarks

This method is avaiable for net4.x versions only.

### See Also

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


