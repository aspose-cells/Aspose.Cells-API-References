##WebExtensionPropertyCollection.Add
WebExtensionPropertyCollection method. Adds web extension property
## WebExtensionPropertyCollection.Add method
Adds web extension property.
```csharp
public int Add(string name, string value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of property. |
| value | String | The value of property. |
### Return Value
The index of added property.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
namespace AsposeCellsExamples
{
public class WebExtensionPropertyCollectionMethodAddWithStringStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
int index = webExtensions.Add();
WebExtension webExt = webExtensions[index];
webExt.Reference.Id = "wa104104476";
webExt.Reference.Version = "1.3.0.0";
webExt.Reference.StoreName = "en-US";
webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
// Demonstrate Add method with (String, String) parameters
webExt.Properties.Add("sku", "peoplebar-giant");
webExt.Properties.Add("theme", "giant-redwhiteblack");
workbook.Save("WebExtensionExample.xlsx");
}
}
}
```
### See Also
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
