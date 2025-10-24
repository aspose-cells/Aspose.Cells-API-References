##ContentTypePropertyCollection.Add
ContentTypePropertyCollection method. Adds content type property information
## Add(string, string) {#add}
Adds content type property information.
```csharp
public int Add(string name, string value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the content type property. |
| value | String | The value of the content type property. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class ContentTypePropertyCollectionMethodAddWithStringStringDemo
{
public static void Run()
{
Workbook wb = new Workbook();
ContentTypePropertyCollection ctps = wb.ContentTypeProperties;
ctps.Add("CustomProperty1", "SampleValue1");
ctps.Add("CustomProperty2", "SampleValue2");
wb.Save("output.xlsx");
}
}
}
```
### See Also
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
## Add(string, string, string) {#add_1}
Adds content type property information.
```csharp
public int Add(string name, string value, string type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the content type property. |
| value | String | The value of the content type property. |
| type | String | The type of the content type property. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ContentTypePropertyCollectionMethodAddWithStringStringStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.ContentTypeProperties.Add("propertyName", "propertyValue", "string");
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
