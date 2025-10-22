##Class Protection
Aspose.Cells.Protection class. Represents the various types of protection options available for a worksheet
## Protection class
Represents the various types of protection options available for a worksheet.
```csharp
public class Protection
```
## Properties
| Name | Description |
| --- | --- |
| [AllowDeletingColumn](../../aspose.cells/protection/allowdeletingcolumn/) { get; set; } | Represents if the deletion of columns is allowed on a protected worksheet. |
| [AllowDeletingRow](../../aspose.cells/protection/allowdeletingrow/) { get; set; } | Represents if the deletion of rows is allowed on a protected worksheet. |
| [AllowEditingContent](../../aspose.cells/protection/alloweditingcontent/) { get; set; } | Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [AllowEditingObject](../../aspose.cells/protection/alloweditingobject/) { get; set; } | Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [AllowEditingScenario](../../aspose.cells/protection/alloweditingscenario/) { get; set; } | Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [AllowFiltering](../../aspose.cells/protection/allowfiltering/) { get; set; } | Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
| [AllowFormattingCell](../../aspose.cells/protection/allowformattingcell/) { get; set; } | Represents if the formatting of cells is allowed on a protected worksheet. |
| [AllowFormattingColumn](../../aspose.cells/protection/allowformattingcolumn/) { get; set; } | Represents if the formatting of columns is allowed on a protected worksheet |
| [AllowFormattingRow](../../aspose.cells/protection/allowformattingrow/) { get; set; } | Represents if the formatting of rows is allowed on a protected worksheet |
| [AllowInsertingColumn](../../aspose.cells/protection/allowinsertingcolumn/) { get; set; } | Represents if the insertion of columns is allowed on a protected worksheet |
| [AllowInsertingHyperlink](../../aspose.cells/protection/allowinsertinghyperlink/) { get; set; } | Represents if the insertion of hyperlinks is allowed on a protected worksheet |
| [AllowInsertingRow](../../aspose.cells/protection/allowinsertingrow/) { get; set; } | Represents if the insertion of rows is allowed on a protected worksheet |
| [AllowSelectingLockedCell](../../aspose.cells/protection/allowselectinglockedcell/) { get; set; } | Represents if the user is allowed to select locked cells on a protected worksheet. |
| [AllowSelectingUnlockedCell](../../aspose.cells/protection/allowselectingunlockedcell/) { get; set; } | Represents if the user is allowed to select unlocked cells on a protected worksheet. |
| [AllowSorting](../../aspose.cells/protection/allowsorting/) { get; set; } | Represents if the sorting option is allowed on a protected worksheet. |
| [AllowUsingPivotTable](../../aspose.cells/protection/allowusingpivottable/) { get; set; } | Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [IsProtectedWithPassword](../../aspose.cells/protection/isprotectedwithpassword/) { get; } | Indicates whether the worksheets is protected with password. |
| [Password](../../aspose.cells/protection/password/) { get; set; } | Represents the password to protect the worksheet. |
## Methods
| Name | Description |
| --- | --- |
| [Copy](../../aspose.cells/protection/copy/)(Protection) | Copy protection info. |
| [GetPasswordHash](../../aspose.cells/protection/getpasswordhash/)() | Gets the hash of current password. |
| [VerifyPassword](../../aspose.cells/protection/verifypassword/)(string) | Verifies password. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ProtectionDemo
{
public static void ProtectionExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Accessing the protection settings of the worksheet
Protection protection = worksheet.Protection;
// Setting various protection properties
protection.AllowDeletingColumn = true;
protection.AllowDeletingRow = true;
protection.AllowFiltering = true;
protection.AllowFormattingCell = true;
protection.AllowFormattingColumn = true;
protection.AllowFormattingRow = true;
protection.AllowInsertingColumn = true;
protection.AllowInsertingHyperlink = true;
protection.AllowInsertingRow = true;
protection.AllowSorting = true;
protection.AllowUsingPivotTable = true;
protection.AllowEditingContent = true;
protection.AllowEditingObject = true;
protection.AllowEditingScenario = true;
protection.Password = "password123";
protection.AllowSelectingLockedCell = true;
protection.AllowSelectingUnlockedCell = true;
// Checking if the worksheet is protected with a password
bool isProtectedWithPassword = protection.IsProtectedWithPassword;
// Saving the workbook
workbook.Save("ProtectionExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
