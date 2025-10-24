##ProtectedRange.Password
ProtectedRange property. Represents the password to protect the range
## ProtectedRange.Password property
Represents the password to protect the range.
```csharp
public string Password { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectedRangePropertyPasswordDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create protected ranges collection
ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;
// Add a protected range
int index = allowRanges.Add("MyProtectedRange", 0, 0, 2, 2);
ProtectedRange protectedRange = allowRanges[index];
// Set password for the protected range
protectedRange.Password = "12345";
// Save the workbook
workbook.Save("ProtectedRangeWithPassword.xlsx");
}
}
}
```
### See Also
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
