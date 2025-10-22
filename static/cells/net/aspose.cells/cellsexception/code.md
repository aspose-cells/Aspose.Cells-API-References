##CellsException.Code
CellsException property. Represents custom exception code
## CellsException.Code property
Represents custom exception code.
```csharp
public ExceptionType Code { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsExceptionPropertyCodeDemo
{
public static void Run()
{
try
{
// Create a workbook and try to access a non-existent worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets["NonExistentSheet"];
}
catch (CellsException e)
{
// Demonstrate usage of the Code property
Console.WriteLine($"Error Code: {e.Code}");
Console.WriteLine($"Error Message: {e.Message}");
}
}
}
}
```
### See Also
* enum [ExceptionType](../../exceptiontype/)
* class [CellsException](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
