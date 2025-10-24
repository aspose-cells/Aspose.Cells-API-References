##XmlLoadOptions.ConvertNumericOrDate
XmlLoadOptions property. Indicates whether converting the value in xml file to numeric or date
## XmlLoadOptions.ConvertNumericOrDate property
Indicates whether converting the value in xml file to numeric or date.
```csharp
public bool ConvertNumericOrDate { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlLoadOptionsPropertyConvertNumericOrDateDemo
{
public static void Run()
{
// Create XML load options
XmlLoadOptions options = new XmlLoadOptions();
// Set ConvertNumericOrDate to true (default)
options.ConvertNumericOrDate = true;
Workbook wb1 = new Workbook("input.xml", options);
Cell cell1 = wb1.Worksheets[0].Cells["A1"];
Console.WriteLine("With conversion (true): " + cell1.Value + " is type: " + cell1.Type);
// Set ConvertNumericOrDate to false
options.ConvertNumericOrDate = false;
Workbook wb2 = new Workbook("input.xml", options);
Cell cell2 = wb2.Worksheets[0].Cells["A1"];
Console.WriteLine("Without conversion (false): " + cell2.Value + " is type: " + cell2.Type);
// Save results
wb1.Save("output_with_conversion.xlsx");
wb2.Save("output_without_conversion.xlsx");
}
}
}
```
### See Also
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
