##Workbook.HasMacro
Workbook property. Indicates if this spreadsheet contains macro/VBA
## Workbook.HasMacro property
Indicates if this spreadsheet contains macro/VBA.
```csharp
public bool HasMacro { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyHasMacroDemo
{
public static void Run()
{
// Create a workbook with macro by loading a template file
Workbook workbookWithMacro = new Workbook("sample_with_macro.xlsm");
Console.WriteLine("Workbook with macro - HasMacro: " + workbookWithMacro.HasMacro);
// Create a workbook without macro
Workbook workbookWithoutMacro = new Workbook();
Console.WriteLine("Workbook without macro - HasMacro: " + workbookWithoutMacro.HasMacro);
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
