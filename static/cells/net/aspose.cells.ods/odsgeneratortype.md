##Enum OdsGeneratorType
Aspose.Cells.Ods.OdsGeneratorType enum. Represents the type of ODS generator
## OdsGeneratorType enumeration
Represents the type of ODS generator.
```csharp
public enum OdsGeneratorType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| LibreOffice | `0` | Libre Office |
| OpenOffice | `1` | Open Office |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;
namespace AsposeCellsExamples
{
public class OdsClassOdsGeneratorTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello World");
OdsSaveOptions saveOptions = new OdsSaveOptions();
saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
workbook.Save("OdsGeneratorTypeDemo.ods", saveOptions);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)
