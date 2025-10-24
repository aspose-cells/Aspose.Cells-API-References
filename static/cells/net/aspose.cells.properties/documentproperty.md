##Class DocumentProperty
Aspose.Cells.Properties.DocumentProperty class. Represents a custom or builtin document property
## DocumentProperty class
Represents a custom or built-in document property.
```csharp
public class DocumentProperty
```
## Properties
| Name | Description |
| --- | --- |
| [IsGeneratedName](../../aspose.cells.properties/documentproperty/isgeneratedname/) { get; } | Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API. |
| [IsLinkedToContent](../../aspose.cells.properties/documentproperty/islinkedtocontent/) { get; } | Indicates whether this property is linked to content |
| [Name](../../aspose.cells.properties/documentproperty/name/) { get; } | Returns the name of the property. |
| [Source](../../aspose.cells.properties/documentproperty/source/) { get; } | The linked content source. |
| [Type](../../aspose.cells.properties/documentproperty/type/) { get; } | Gets the data type of the property. |
| [Value](../../aspose.cells.properties/documentproperty/value/) { get; set; } | Gets or sets the value of the property. |
## Methods
| Name | Description |
| --- | --- |
| [ToBool](../../aspose.cells.properties/documentproperty/tobool/)() | Returns the property value as bool. |
| [ToDateTime](../../aspose.cells.properties/documentproperty/todatetime/)() | Returns the property value as DateTime in local timezone. |
| [ToDouble](../../aspose.cells.properties/documentproperty/todouble/)() | Returns the property value as double. |
| [ToInt](../../aspose.cells.properties/documentproperty/toint/)() | Returns the property value as integer. |
| override [ToString](../../aspose.cells.properties/documentproperty/tostring/)() | Returns the property value as a string. |
### Examples
```csharp
[C#]
//Instantiate a Workbook object
Workbook workbook = new Workbook("book1.xls");
//Retrieve a list of all custom document properties of the Excel file
DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
//Accessng a custom document property by using the property index
DocumentProperty customProperty1 = customProperties[3];
//Accessng a custom document property by using the property name
DocumentProperty customProperty2 = customProperties["Owner"];
[VB.NET]
'Instantiate a Workbook object
Dim workbook As Workbook = New Workbook("book1.xls")
'Retrieve a list of all custom document properties of the Excel file
Dim customProperties As DocumentPropertyCollection = workbook.Worksheets.CustomDocumentProperties
'Accessng a custom document property by using the property index
Dim customProperty1 As DocumentProperty = customProperties(3)
'Accessng a custom document property by using the property name
Dim customProperty2 As DocumentProperty = customProperties("Owner")
```
### See Also
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)
