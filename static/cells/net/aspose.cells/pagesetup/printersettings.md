##PageSetup.PrinterSettings
PageSetup property. Gets and sets the settings of the default printer
## PageSetup.PrinterSettings property
Gets and sets the settings of the default printer.
```csharp
public byte[] PrinterSettings { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyPrinterSettingsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells["A1"].PutValue("Test Printer Settings");
// Access page setup
PageSetup pageSetup = worksheet.PageSetup;
// Set printer settings (as byte array)
byte[] printerSettings = new byte[10]; // Simplified example
pageSetup.PrinterSettings = printerSettings;
// Verify printer settings are set
Console.WriteLine("Printer Settings: " + (pageSetup.PrinterSettings != null));
// Save the workbook
workbook.Save("PrinterSettingsDemo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
