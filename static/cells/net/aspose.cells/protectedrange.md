##Class ProtectedRange
Aspose.Cells.ProtectedRange class. A specified range to be allowed to edit when the sheet protection is ON
## ProtectedRange class
A specified range to be allowed to edit when the sheet protection is ON.
```csharp
public class ProtectedRange
```
## Properties
| Name | Description |
| --- | --- |
| [CellArea](../../aspose.cells/protectedrange/cellarea/) { get; } | Gets the [`CellArea`](./cellarea/) object represents the cell area to be protected. |
| [IsProtectedWithPassword](../../aspose.cells/protectedrange/isprotectedwithpassword/) { get; } | Indicates whether the worksheets is protected with password. |
| [Name](../../aspose.cells/protectedrange/name/) { get; set; } | Gets the Range title. This is used as a descriptor, not as a named range definition. |
| [Password](../../aspose.cells/protectedrange/password/) { get; set; } | Represents the password to protect the range. |
| [SecurityDescriptor](../../aspose.cells/protectedrange/securitydescriptor/) { get; set; } | The security descriptor defines user accounts who may edit this range without providing a password to access the range. |
## Methods
| Name | Description |
| --- | --- |
| [AddArea](../../aspose.cells/protectedrange/addarea/)(int, int, int, int) | Adds a referred area to this |
| [GetAreas](../../aspose.cells/protectedrange/getareas/)() | Gets all referred areas. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassProtectedRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Get the collection of protected ranges
ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
// Add a new protected range (A1:J10)
int index = protectedRanges.Add("MyProtectedRange", 0, 0, 10, 10);
// Get the protected range
ProtectedRange protectedRange = protectedRanges[index];
// Set security descriptor
string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
protectedRange.SecurityDescriptor = securityDescriptor;
// Save the workbook
workbook.Save("ProtectedRangeDemo.xlsx");
Console.WriteLine("Protected range demo completed successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
