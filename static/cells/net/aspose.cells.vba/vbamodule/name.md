##VbaModule.Name
VbaModule property. Gets and sets the name of Module
## VbaModule.Name property
Gets and sets the name of Module.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaModulePropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Add a worksheet and get its VBA module
Worksheet sheet = wb.Worksheets[0];
int moduleIndex = wb.VbaProject.Modules.Add(sheet);
VbaModule module = wb.VbaProject.Modules[moduleIndex];
// Set the module name
module.Name = "Sheet1";
// Add simple VBA code to the module
string vbaCode = "Private Sub Worksheet_SelectionChange(ByVal Target As Range)\r\n" +
"    MsgBox \"Sheet name: \" & Me.Name\r\n" +
"End Sub\r\n";
module.Codes = vbaCode;
// Save to memory stream (for demonstration)
using (MemoryStream ms = new MemoryStream())
{
wb.Save(ms, SaveFormat.Xlsm);
}
}
}
}
```
### See Also
* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
