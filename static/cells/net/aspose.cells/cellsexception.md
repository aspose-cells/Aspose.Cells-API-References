##Class CellsException
Aspose.Cells.CellsException class. The exception that is thrown when Aspose.Cells specified error occurs
## CellsException class
The exception that is thrown when Aspose.Cells specified error occurs.
```csharp
public class CellsException : ApplicationException
```
## Properties
| Name | Description |
| --- | --- |
| [Code](../../aspose.cells/cellsexception/code/) { get; } | Represents custom exception code. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Reflection;
using System.Collections;
public class CellsExceptionDemo
{
public static void CellsExceptionExample()
{
try
{
// Simulate an operation that causes an exception
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Intentionally causing an exception by accessing an invalid cell
Cell cell = worksheet.Cells["InvalidCellAddress"];
}
catch (CellsException ex)
{
// Handle the CellsException
Console.WriteLine("Aspose.Cells.CellsException caught!");
Console.WriteLine($"Code: {ex.Code}");
Console.WriteLine($"Message: {ex.Message}");
Console.WriteLine($"TargetSite: {ex.TargetSite}");
Console.WriteLine($"StackTrace: {ex.StackTrace}");
Console.WriteLine($"HelpLink: {ex.HelpLink}");
Console.WriteLine($"Source: {ex.Source}");
Console.WriteLine($"HResult: {ex.HResult}");
if (ex.InnerException != null)
{
Console.WriteLine($"InnerException: {ex.InnerException.Message}");
}
foreach (DictionaryEntry entry in ex.Data)
{
Console.WriteLine($"Data: {entry.Key} = {entry.Value}");
}
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
