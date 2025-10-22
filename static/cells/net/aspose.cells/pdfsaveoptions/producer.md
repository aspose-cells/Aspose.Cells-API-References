##PdfSaveOptions.Producer
PdfSaveOptions property. Gets and sets producer of generated pdf document
## PdfSaveOptions.Producer property
Gets and sets producer of generated pdf document.
```csharp
public string Producer { get; set; }
```
### Remarks
If the value is null, or a valid LICENSE is not set, string Aspose.Cells vVERSION will be used.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsPropertyProducerDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet and add sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("PDF Producer Property Demo");
// Create PDF save options
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Set the Producer property
pdfSaveOptions.Producer = "Aspose.Cells for .NET";
// Save to memory stream
using (MemoryStream stream = new MemoryStream())
{
workbook.Save(stream, pdfSaveOptions);
// Verify the Producer was set
stream.Position = 0;
using (StreamReader reader = new StreamReader(stream))
{
string content = reader.ReadToEnd();
Console.WriteLine(content.Contains("/Producer (Aspose.Cells for .NET)")
? "Producer property set successfully"
: "Failed to set Producer property");
}
}
}
}
}
```
### See Also
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
