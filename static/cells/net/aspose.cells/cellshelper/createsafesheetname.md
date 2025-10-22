##CellsHelper.CreateSafeSheetName
CellsHelper method. Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with   then return the rebuilt string value
## CreateSafeSheetName(string) {#createsafesheetname}
Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with ' ', then return the rebuilt string value.
```csharp
public static string CreateSafeSheetName(string nameProposal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| nameProposal | String | sheet name to be used |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperMethodCreateSafeSheetNameWithStringDemo
{
public static void Run()
{
string unsafeName = "sheet*/test*/?#";
string safeName = CellsHelper.CreateSafeSheetName(unsafeName);
Console.WriteLine("Original name: " + unsafeName);
Console.WriteLine("Safe name: " + safeName);
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CreateSafeSheetName(string, char) {#createsafesheetname_1}
Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with given character, then return the rebuilt string value.
```csharp
public static string CreateSafeSheetName(string nameProposal, char replaceChar)
```
| Parameter | Type | Description |
| --- | --- | --- |
| nameProposal | String | sheet name to be used |
| replaceChar | Char | character which will be used to replace invalid characters in given sheet name |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperMethodCreateSafeSheetNameWithStringCharDemo
{
public static void Run()
{
// Example 1: Create safe sheet name with default replacement character
string name1 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#");
Console.WriteLine("Safe sheet name (default replacement): " + name1);
// Example 2: Create safe sheet name with custom replacement character 'A'
string name2 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#", 'A');
Console.WriteLine("Safe sheet name (custom replacement): " + name2);
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
