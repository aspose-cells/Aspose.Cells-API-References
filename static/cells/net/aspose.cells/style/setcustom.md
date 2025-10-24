##Style.SetCustom
Style method. Sets the Custom number format string of a cell
## Style.SetCustom method
Sets the Custom number format string of a cell.
```csharp
public void SetCustom(string custom, bool builtinPreference)
```
| Parameter | Type | Description |
| --- | --- | --- |
| custom | String | Custom number format string, should be InvariantCulture pattern. |
| builtinPreference | Boolean | If given Custom number format string matches one of the built-in number formats corresponding to current regional settings, whether set the number format as built-in instead of Custom. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleMethodSetCustomWithStringBooleanDemo
{
public static void Run()
{
Workbook wb = new Workbook();
wb.Settings.Region = CountryCode.USA;
Style style = wb.CreateStyle();
string customFormat1 = "_(\"$\"* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
style.SetCustom(customFormat1, true);
Console.WriteLine("Custom format 1 applied. Style number: " + style.Number);
string customFormat2 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
style.SetCustom(customFormat2, true);
Console.WriteLine("Custom format 2 applied. Style number: " + style.Number);
string customFormat3 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* -??_);_(@_)";
style.SetCustom(customFormat3, true);
Console.WriteLine("Custom format 3 applied. Style number: " + style.Number);
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
