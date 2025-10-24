##OdsSaveOptions.GeneratorType
OdsSaveOptions property. Gets and sets the generator of the ods file
## OdsSaveOptions.GeneratorType property
Gets and sets the generator of the ods file.
```csharp
public OdsGeneratorType GeneratorType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;
namespace AsposeCellsExamples
{
public class OdsSaveOptionsPropertyGeneratorTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello World");
// Create and configure ODS save options
OdsSaveOptions saveOptions = new OdsSaveOptions
{
GeneratorType = OdsGeneratorType.LibreOffice,
IsStrictSchema11 = true
};
// Save the workbook with specified options
workbook.Save("OdsSaveOptions_GeneratorTypeDemo.ods", saveOptions);
}
}
}
```
### See Also
* enum [OdsGeneratorType](../../../aspose.cells.ods/odsgeneratortype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
