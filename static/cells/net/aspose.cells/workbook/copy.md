##Workbook.Copy
Workbook method. Copies another Workbook object
## Copy(Workbook, CopyOptions) {#copy_1}
Copies another Workbook object.
```csharp
public void Copy(Workbook source, CopyOptions copyOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | Source Workbook object. |
| copyOptions | CopyOptions | The options of copying other workbook. |
### Remarks
It's very simple to clone an Excel file.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCopyWithWorkbookCopyOptionsDemo
{
public static void Run()
{
// Source workbook with macros
Workbook sourceWorkbook = new Workbook("source_with_macros.xlsm");
// Destination workbook (empty or existing)
Workbook destWorkbook = new Workbook();
// Configure copy options to keep macros
CopyOptions options = new CopyOptions();
options.KeepMacros = true;
// Copy contents from source to destination workbook
sourceWorkbook.Copy(destWorkbook, options);
// Save the result
destWorkbook.Save("output_with_macros.xlsm");
}
}
}
```
### See Also
* class [CopyOptions](../../copyoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Copy(Workbook) {#copy}
Copies data from a source Workbook object.
```csharp
public void Copy(Workbook source)
```
| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | Source Workbook object. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCopyWithWorkbookDemo
{
public static void Run()
{
// Source and output file paths
string sourceFile = "source.xlsx";
string outputFile = "output.xlsx";
// Load the source workbook
Workbook sourceWorkbook = new Workbook(sourceFile);
// Create a new workbook and copy contents from source
Workbook destinationWorkbook = new Workbook();
destinationWorkbook.Copy(sourceWorkbook);
// Save the copied workbook
destinationWorkbook.Save(outputFile);
Console.WriteLine("Workbook copied successfully.");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
