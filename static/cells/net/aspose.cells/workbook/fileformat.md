##Workbook.FileFormat
Workbook property. Gets and sets the file format
## Workbook.FileFormat property
Gets and sets the file format.
```csharp
public FileFormatType FileFormat { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyFileFormatDemo
{
public static void Run()
{
// Create a sample CSV file
string csvFile = "sample.csv";
File.WriteAllText(csvFile, "Name,Age\nJohn,30\nJane,25");
// Create a sample XLSX file
string xlsxFile = "sample.xlsx";
using (Workbook wb = new Workbook())
{
wb.Worksheets[0].Cells["A1"].PutValue("Test");
wb.Save(xlsxFile);
}
// Demonstrate FileFormat property
ProcessWorkbook(csvFile);
ProcessWorkbook(xlsxFile);
// Cleanup
File.Delete(csvFile);
File.Delete(xlsxFile);
}
private static void ProcessWorkbook(string filePath)
{
using (Workbook wb = new Workbook(filePath))
{
Console.WriteLine($"Processing file: {filePath}");
Console.WriteLine($"File format: {wb.FileFormat}");
if (wb.FileFormat == FileFormatType.Csv)
{
Console.WriteLine("This is a CSV file");
// Additional CSV-specific processing
}
else if (wb.FileFormat == FileFormatType.Xlsx)
{
Console.WriteLine("This is an XLSX file");
// Additional XLSX-specific processing
}
}
}
}
}
```
### See Also
* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
