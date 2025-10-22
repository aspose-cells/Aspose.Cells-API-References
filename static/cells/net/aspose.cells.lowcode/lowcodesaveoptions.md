##Class LowCodeSaveOptions
Aspose.Cells.LowCode.LowCodeSaveOptions class. Options for saving generated results in low code way
## LowCodeSaveOptions class
Options for saving generated results in low code way.
```csharp
public class LowCodeSaveOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [LowCodeSaveOptions](lowcodesaveoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [`OutputStream`](./outputstream/) will be ignored. |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [`OutputFile`](./outputfile/) will be ignored. |
| virtual [SaveFormat](../../aspose.cells.lowcode/lowcodesaveoptions/saveformat/) { get; set; } | Gets and sets the save format for the output. Generally, for specific process in low code way, only some specific formats are allowed. Please specify the correct format for corresponding process, otherwise unexpected result or even exception may be caused. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
namespace AsposeCellsExamples
{
public class LowCodeClassLowCodeSaveOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and put some data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello");
worksheet.Cells["B1"].PutValue("World");
// Create save options
LowCodeSaveOptions saveOptions = new LowCodeSaveOptions()
{
OutputFile = "output.xlsx"
};
// Save the workbook using the specified options
workbook.Save(saveOptions.OutputFile, saveOptions.SaveFormat);
Console.WriteLine("File saved successfully with LowCodeSaveOptions");
}
}
}
```
### See Also
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)
