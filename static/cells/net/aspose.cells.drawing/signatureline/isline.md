##SignatureLine.IsLine
SignatureLine property. Indicates whether it is a signature line
## SignatureLine.IsLine property
Indicates whether it is a signature line.
```csharp
public bool IsLine { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class SignatureLinePropertyIsLineDemo
{
public static void Run()
{
// Create a signature line instance
SignatureLine signature = new SignatureLine();
// Set IsLine to true
signature.IsLine = true;
// Check and demonstrate IsLine usage
if (signature.IsLine)
{
Console.WriteLine("Signature line is active.");
}
// Toggle IsLine state
signature.IsLine = false;
if (!signature.IsLine)
{
Console.WriteLine("Signature line is now inactive.");
}
}
}
}
```
### See Also
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
