##Class ContentTypeProperty
Aspose.Cells.Properties.ContentTypeProperty class. Represents identifier information
## ContentTypeProperty class
Represents identifier information.
```csharp
public class ContentTypeProperty
```
## Properties
| Name | Description |
| --- | --- |
| [IsNillable](../../aspose.cells.properties/contenttypeproperty/isnillable/) { get; set; } | Indicates whether the value could be empty. |
| [Name](../../aspose.cells.properties/contenttypeproperty/name/) { get; set; } | Returns or sets the name of the object. |
| [Type](../../aspose.cells.properties/contenttypeproperty/type/) { get; set; } | Gets and sets the type of the property. |
| [Value](../../aspose.cells.properties/contenttypeproperty/value/) { get; set; } | Returns or sets the value of the content type property. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Properties;
using System;
public class ContentTypePropertyDemo
{
public static void ContentTypePropertyExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Add a new content type property
workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
// Access the newly added property
ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
// Setting properties
property.Name = "Admin";
property.Value = "Aspose";
property.Type = "text";
property.IsNillable = true;
// Save the Excel file
workbook.Save("ContentTypePropertyExample.xlsx");
workbook.Save("ContentTypePropertyExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)
