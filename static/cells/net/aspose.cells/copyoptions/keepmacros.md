##CopyOptions.KeepMacros
CopyOptions property. Indicates whether keeping macros
## CopyOptions.KeepMacros property
Indicates whether keeping macros;
```csharp
public bool KeepMacros { get; set; }
```
### Remarks
Only for copying workbook.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CopyOptionsPropertyKeepMacrosDemo
{
public static void Run()
{
// Create source workbook with macros (using a template file that contains macros)
Workbook srcWorkbook = new Workbook("macros_template.xlsm");
Worksheet srcSheet = srcWorkbook.Worksheets[0];
srcSheet.Cells["A1"].PutValue("Macro-enabled source");
// Create destination workbook
Workbook destWorkbook = new Workbook();
// Set copy options with KeepMacros true
CopyOptions options = new CopyOptions();
options.KeepMacros = true;
// Copy worksheet with macros
destWorkbook.Worksheets[0].Copy(srcSheet, options);
// Save result
destWorkbook.Save("KeepMacrosExample.xlsm");
}
}
}
```
### See Also
* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
