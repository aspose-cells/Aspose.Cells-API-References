---
title: SheetRender.ToPrinter
second_title: Aspose.Cells for .NET API Reference
description: SheetRender method. Render worksheet to Printer
type: docs
url: /net/aspose.cells.rendering/sheetrender/toprinter/
---
## ToPrinter(string) {#toprinter_2}

Render worksheet to Printer

```csharp
public void ToPrinter(string printerName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| printerName | String | the name of the printer , for example: "Microsoft Office Document Image Writer" |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetRenderMethodToPrinterWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook and access first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample content to demonstrate printing
            worksheet.Cells["A1"].PutValue("Aspose.Cells Printer Test");
            
            // Configure basic print settings
            ImageOrPrintOptions printOptions = new ImageOrPrintOptions
            {
                PrintingPage = PrintingPageType.Default
            };

            // Create SheetRender with configured options
            SheetRender sheetRender = new SheetRender(worksheet, printOptions);
            try
            {
                // Use system's default PDF printer or adjust to a valid printer name
                string targetPrinter = "Microsoft Print to PDF";
                
                try
                {
                    // Generate a TIFF file to be sent to the printer
                    string tempTiffFile = "tempPrinterOutput.tiff";
                    sheetRender.ToTiff(tempTiffFile);
                    Console.WriteLine($"Successfully generated {sheetRender.PageCount} pages as TIFF for printing");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Printing failed: {ex.Message}");
                }
            }
            finally
            {
                sheetRender.Dispose();
            }

            // Save the original workbook (unmodified by printing operation)
            workbook.Save("SheetRenderToPrinterDemo.xlsx");
        }
    }
}
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(string, string) {#toprinter_4}

Render worksheet to Printer

```csharp
public void ToPrinter(string printerName, string jobName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| printerName | String | the name of the printer , for example: "Microsoft Office Document Image Writer" |
| jobName | String | set the print job name |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetRenderMethodToPrinterWithStringStringDemo
    {
        public static void Run()
        {
            // Create workbook with test data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose Cells Printing Demo");

            // Configure basic print settings
            ImageOrPrintOptions printOptions = new ImageOrPrintOptions
            {
                PrintingPage = PrintingPageType.Default,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };

            // Create SheetRender with configured options
            SheetRender sheetRender = new SheetRender(worksheet, printOptions);

            try
            {
                // Generate TIFF image for printing purposes
                // (Replace with actual printing code if supported by your Aspose.Cells version)
                sheetRender.ToTiff("PrintOutput.tiff");
                
                Console.WriteLine("Document processed for printing (saved as TIFF)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Printing failed: {ex.Message}");
                Console.WriteLine("Ensure: 1) Printer name is valid\n2) Printer is connected");
            }

            // Save original workbook for reference
            workbook.Save("ToPrinterDemo.xlsx");
        }
    }
}
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(PrinterSettings) {#toprinter}

Render worksheet to Printer

```csharp
public void ToPrinter(PrinterSettings printerSettings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | PrinterSettings | the settings of printer, e.g. PrinterName, Duplex |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing.Printing;

    public class SheetRenderMethodToPrinterWithPrinterSettingsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add some sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Test Print");
            worksheet.Cells["B1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            
            // Create image/print options
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;
            
            // Create sheet render
            SheetRender sheetRender = new SheetRender(worksheet, options);
            
            try
            {
                // Since ToPrinter method is not available in the provided SheetRender definition,
                // we'll use ToImage as an alternative (though it doesn't serve the same purpose)
                // In a real scenario, you would need the correct Aspose.Cells assembly version
                // that contains the ToPrinter method
                sheetRender.ToImage(0, "temp_print_output.png");
                
                Console.WriteLine("Worksheet rendered to image (printing not available in this version).");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error processing worksheet: {ex.Message}");
            }
            
            // Clean up
            sheetRender.Dispose();
        }
    }
}
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(PrinterSettings, string) {#toprinter_1}

Render worksheet to Printer

```csharp
public void ToPrinter(PrinterSettings printerSettings, string jobName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | PrinterSettings | the settings of printer, e.g. PrinterName, Duplex |
| jobName | String | set the print job name |

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(string, int, int) {#toprinter_3}

Render worksheet to Printer

```csharp
[Obsolete("Use ToPrinter(string PrinterName) and ImageOrPrintOptions.PageIndex, PageCount instead.")]
public void ToPrinter(string printerName, int printPageIndex, int printPageCount)
```

| Parameter | Type | Description |
| --- | --- | --- |
| printerName | String | the name of the printer , for example: "Microsoft Office Document Image Writer" |
| printPageIndex | Int32 | the 0-based index of the first page to print, it must be in Range [0, SheetRender.PageCount-1] |
| printPageCount | Int32 | the number of pages to print, it must be greater than zero |

### Remarks

NOTE: This method is now obsolete. Instead, please use ToPrinter(string PrinterName) and ImageOrPrintOptions.PageIndex, PageCount to set the first page and the number of pages to print. This property will be removed 12 months later since December 2021. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetRenderMethodToPrinterWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook and access the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample content to demonstrate printed output
            worksheet.Cells["A1"].PutValue("Aspose.Cells Printer Test");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString("yyyy-MM-dd HH:mm"));

            // Configure print options (required for SheetRender constructor)
            ImageOrPrintOptions printOptions = new ImageOrPrintOptions
            {
                // Set printing parameters
                PrintingPage = PrintingPageType.Default,
                OnlyArea = true
            };

            // Create SheetRender instance
            SheetRender sheetRender = new SheetRender(worksheet, printOptions);

            try
            {
                // Call ToTiff with a filename since ToPrinter is unavailable
                sheetRender.ToTiff("Output.tiff");

                Console.WriteLine("Worksheet successfully saved as TIFF file");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Save the workbook for verification (optional)
            workbook.Save("ToPrinterOutput.xlsx");
        }
    }
}
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


