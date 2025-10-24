##Class Validation
Aspose.Cells.GridWeb.Validation class.
## Validation class
```csharp
[Obsolete("This class is obsolete; use  GridValidation instead")]
public class Validation : CellAttachObject
```
## Constructors
| Name | Description |
| --- | --- |
| [Validation](validation/#constructor)() | The default constructor. |
| [Validation](validation/#constructor_1)(GridValidation) |  |
## Properties
| Name | Description |
| --- | --- |
| [Cell](../../aspose.cells.gridweb.data/cellattachobject/cell/) { get; } | Gets the relative cell of the object.(Inherited from [`CellAttachObject`](../../aspose.cells.gridweb.data/cellattachobject/).) |
| [ClientValidationFunction](../../aspose.cells.gridweb/validation/clientvalidationfunction/) { get; set; } | Gets or sets the client validation javascript function name. |
| [ClientValidationOpType](../../aspose.cells.gridweb/validation/clientvalidationoptype/) { get; set; } | Gets or sets the validation op type ,Between/NotBetween/Equal/NotEqual/Greater/GreaterOrEqual/Less/LessOrEqual. |
| [ClientValidationValue1](../../aspose.cells.gridweb/validation/clientvalidationvalue1/) { get; set; } | Gets or sets the operator target value 1 |
| [ClientValidationValue2](../../aspose.cells.gridweb/validation/clientvalidationvalue2/) { get; set; } | Gets or sets the operator target value 2 |
| [IsRequired](../../aspose.cells.gridweb/validation/isrequired/) { get; set; } | Gets or sets whether the cell value is required. |
| [RegEx](../../aspose.cells.gridweb/validation/regex/) { get; set; } | Gets or sets the regular expression string. |
| [ValueArray](../../aspose.cells.gridweb/validation/valuearray/) { get; set; } |  |
| [ValueList](../../aspose.cells.gridweb/validation/valuelist/) { get; } | Gets the value list object. |
| [ValueText](../../aspose.cells.gridweb/validation/valuetext/) { get; set; } | Design time used only. |
## Methods
| Name | Description |
| --- | --- |
| [LoadValueList](../../aspose.cells.gridweb/validation/loadvaluelist/)(DataView, string, string, bool) | Loads value list from a DataView object. You can specify the value field and text field of the DataView. Each value and text pair will be combined to one string, with a comma between them. |
### Remarks
NOTE: This class is now obsolete. please use GridValidation Instead. This class will be removed after 6 months since Aug. 2014. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* class [CellAttachObject](../../aspose.cells.gridweb.data/cellattachobject/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)
