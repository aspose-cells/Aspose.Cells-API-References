##Workbook.RemoveMacro
Workbook method. Removes VBA/macro from this spreadsheet
## Workbook.RemoveMacro method
Removes VBA/macro from this spreadsheet.
```csharp
public void RemoveMacro()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodRemoveMacroDemo
{
public static void Run()
{
// Create a workbook from an existing macro-enabled file
Workbook workbook = new Workbook("example.xlsm");
// Remove macros from the workbook
workbook.RemoveMacro();
// Save as macro-free workbook
string noMacroPath = "NoMacro.xlsx";
workbook.Save(noMacroPath, SaveFormat.Xlsx);
Console.WriteLine("Macros removed successfully. File created: " + noMacroPath);
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
