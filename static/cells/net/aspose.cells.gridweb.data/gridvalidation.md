##Class GridValidation
Aspose.Cells.GridWeb.Data.GridValidation class. Represents data validation.settings
## GridValidation class
Represents data validation.settings.
```csharp
public class GridValidation
```
## Properties
| Name | Description |
| --- | --- |
| [AreaList](../../aspose.cells.gridweb.data/gridvalidation/arealist/) { get; } | Represents a collection of [`GridCellArea`](../gridcellarea/) which contains the data validation settings. |
| [ClientValidationFunction](../../aspose.cells.gridweb.data/gridvalidation/clientvalidationfunction/) { get; set; } | Gets or sets the client validation javascript function name. |
| [ErrorMessage](../../aspose.cells.gridweb.data/gridvalidation/errormessage/) { get; set; } | Represents the data validation error message. |
| [ErrorTitle](../../aspose.cells.gridweb.data/gridvalidation/errortitle/) { get; set; } | Represents the title of the data-validation error dialog box. |
| [Formula1](../../aspose.cells.gridweb.data/gridvalidation/formula1/) { get; set; } | Represents the value or expression associated with the data validation. |
| [Formula2](../../aspose.cells.gridweb.data/gridvalidation/formula2/) { get; set; } | Represents the value or expression associated with the second part of the data validation. |
| [InputMessage](../../aspose.cells.gridweb.data/gridvalidation/inputmessage/) { get; set; } | Represents the data validation error message. |
| [InputTitle](../../aspose.cells.gridweb.data/gridvalidation/inputtitle/) { get; set; } | Represents the title of the data-validation input dialog box. |
| [IsRequired](../../aspose.cells.gridweb.data/gridvalidation/isrequired/) { get; set; } | Gets or sets whether the cell value is required. |
| [Operator](../../aspose.cells.gridweb.data/gridvalidation/operator/) { get; set; } | Represents the operator for the data validation. |
| [RegEx](../../aspose.cells.gridweb.data/gridvalidation/regex/) { get; set; } | Gets or sets the regular expression string. |
| [ShowError](../../aspose.cells.gridweb.data/gridvalidation/showerror/) { get; set; } | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [ShowInput](../../aspose.cells.gridweb.data/gridvalidation/showinput/) { get; set; } | Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range. |
| [ValidationType](../../aspose.cells.gridweb.data/gridvalidation/validationtype/) { get; set; } | Gets or sets the validation type. |
| [Value1](../../aspose.cells.gridweb.data/gridvalidation/value1/) { get; } | Represents the value associated with the data validation. |
| [ValueList](../../aspose.cells.gridweb.data/gridvalidation/valuelist/) { get; set; } | Gets/Sets the value list object. |
## Methods
| Name | Description |
| --- | --- |
| [AddACell](../../aspose.cells.gridweb.data/gridvalidation/addacell/#addacell_1)(string) | add the validation settings in the cell. |
| [AddACell](../../aspose.cells.gridweb.data/gridvalidation/addacell/#addacell)(int, int) | add the validation settings in the cell. |
| [AddArea](../../aspose.cells.gridweb.data/gridvalidation/addarea/)(GridCellArea) | Applies the validation to the area. |
| [GetListValue](../../aspose.cells.gridweb.data/gridvalidation/getlistvalue/)(int, int) | Get the value for list of the validation for the specified cell. |
| [LoadValueList](../../aspose.cells.gridweb.data/gridvalidation/loadvaluelist/)(DataView, string, string, bool) | Loads value list from a DataView object. You can specify the value field and text field of the DataView. Each value and text pair will be combined to one string, with a comma between them. |
| [RemoveACell](../../aspose.cells.gridweb.data/gridvalidation/removeacell/)(int, int) | Remove the validation settings in the cell. |
| [RemoveArea](../../aspose.cells.gridweb.data/gridvalidation/removearea/)(GridCellArea) | Remove the validation settings in the range. |
## Fields
| Name | Description |
| --- | --- |
| [ServerValidation](../../aspose.cells.gridweb.data/gridvalidation/servervalidation/) | Gets or sets the serverside validation javascript function name. |
### See Also
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
