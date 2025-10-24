##LowCodeSaveOptionsProviderOfPlaceHolders.LowCodeSaveOptionsProviderOfPlaceHolders
LowCodeSaveOptionsProviderOfPlaceHolders constructor. Instantiates an instance to provide save options according to specified templates
## LowCodeSaveOptionsProviderOfPlaceHolders constructor
Instantiates an instance to provide save options according to specified templates.
```csharp
public LowCodeSaveOptionsProviderOfPlaceHolders(string pathTemplate)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pathTemplate | String | The template of the resultant file path. |
### Remarks
The supported placeholders in file path template: ${SheetIndex}: will be replaced by the sheet index of the split part${SheetName}: will be replaced by the sheet name of the split part${SplitPartIndex}: will be replaced by the index of the split part${SheetIndexPrefix}: will be replaced by [`SheetIndexPrefix`](../sheetindexprefix/)${SheetNamePrefix}: will be replaced by [`SheetNamePrefix`](../sheetnameprefix/)${SplitPartPrefix}: will be replaced by [`SplitPartPrefix`](../splitpartprefix/)
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeSaveOptionsProviderOfPlaceHoldersMethodCtorWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Call the #ctor method with String parameter
string pathTemplate = "output_{sheet}_part_{part}.xlsx";
var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);
// Set some properties
provider.SheetIndexOffset = 0;
provider.SplitPartIndexOffset = 0;
provider.SheetNamePrefix = "Sheet_";
provider.SplitPartPrefix = "Part_";
Console.WriteLine("LowCodeSaveOptionsProviderOfPlaceHolders created successfully with path template: " + pathTemplate);
Console.WriteLine($"SheetNamePrefix: {provider.SheetNamePrefix}, SplitPartPrefix: {provider.SplitPartPrefix}");
}
catch (Exception ex)
{
Console.WriteLine($"Error creating LowCodeSaveOptionsProviderOfPlaceHolders: {ex.Message}");
}
// Save the workbook
workbook.Save("LowCodeSaveOptionsProviderDemo.xlsx");
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
