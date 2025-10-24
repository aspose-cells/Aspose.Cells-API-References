##Class Validation
Aspose.Cells.Validation class. Represents data validation.settings
## Validation class
Represents data validation.settings.
```csharp
public class Validation
```
## Properties
| Name | Description |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle/) { get; set; } | Represents the validation alert style. |
| [Areas](../../aspose.cells/validation/areas/) { get; } | Gets all [`CellArea`](../cellarea/) which contain the data validation settings. |
| [ErrorMessage](../../aspose.cells/validation/errormessage/) { get; set; } | Represents the data validation error message. |
| [ErrorTitle](../../aspose.cells/validation/errortitle/) { get; set; } | Represents the title of the data-validation error dialog box. |
| [Formula1](../../aspose.cells/validation/formula1/) { get; set; } | Represents the value or expression associated with the data validation. |
| [Formula2](../../aspose.cells/validation/formula2/) { get; set; } | Represents the value or expression associated with the data validation. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank/) { get; set; } | Indicates whether blank values are permitted by the range data validation. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown/) { get; set; } | Indicates whether data validation displays a drop-down list that contains acceptable values. |
| [InputMessage](../../aspose.cells/validation/inputmessage/) { get; set; } | Represents the data validation input message. |
| [InputTitle](../../aspose.cells/validation/inputtitle/) { get; set; } | Represents the title of the data-validation input dialog box. |
| [Operator](../../aspose.cells/validation/operator/) { get; set; } | Represents the operator for the data validation. |
| [ShowError](../../aspose.cells/validation/showerror/) { get; set; } | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [ShowInput](../../aspose.cells/validation/showinput/) { get; set; } | Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range. |
| [Type](../../aspose.cells/validation/type/) { get; set; } | Represents the data validation type. |
| [Value1](../../aspose.cells/validation/value1/) { get; set; } | Represents the first value associated with the data validation. |
| [Value2](../../aspose.cells/validation/value2/) { get; set; } | Represents the second value associated with the data validation. |
## Methods
| Name | Description |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea/#addarea)(CellArea) | Applies the validation to the area. |
| [AddArea](../../aspose.cells/validation/addarea/#addarea_1)(CellArea, bool, bool) | Applies the validation to the area. |
| [AddAreas](../../aspose.cells/validation/addareas/)(CellArea[], bool, bool) | Applies the validation to given areas. |
| [Copy](../../aspose.cells/validation/copy/)(Validation, CopyOptions) | Copy validation. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1)(bool, bool) | Gets the value or expression associated with this validation. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1_1)(bool, bool, int, int) | Gets the value or expression associated with this validation for specific cell. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2)(bool, bool) | Gets the value or expression associated with this validation. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2_1)(bool, bool, int, int) | Gets the value or expression associated with this validation for specific cell. |
| [GetListValue](../../aspose.cells/validation/getlistvalue/)(int, int) | Get the value for list of the validation for the specified cell. |
| [GetValue](../../aspose.cells/validation/getvalue/)(int, int, bool) | Get the value of validation on the specific cell. |
| [RemoveACell](../../aspose.cells/validation/removeacell/)(int, int) | Remove the validation settings in the cell. |
| [RemoveArea](../../aspose.cells/validation/removearea/)(CellArea) | Remove the validation settings in the range. |
| [RemoveAreas](../../aspose.cells/validation/removeareas/)(CellArea[]) | Removes this validation from given areas. |
| [SetFormula1](../../aspose.cells/validation/setformula1/)(string, bool, bool) | Sets the value or expression associated with this validation. |
| [SetFormula2](../../aspose.cells/validation/setformula2/)(string, bool, bool) | Sets the value or expression associated with this validation. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ValidationDemo
{
public static void ValidationExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Define a cell area for the validation
CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
// Access the validations collection
ValidationCollection validations = worksheet.Validations;
// Add a new validation to the collection
int validationIndex = validations.Add(area);
Validation validation = validations[validationIndex];
// Set validation properties
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "3";
validation.Formula2 = "1234";
validation.InputMessage = "Please enter a whole number between 3 and 1234.";
validation.InputTitle = "Whole Number Validation";
validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
validation.ErrorTitle = "Invalid Input";
validation.ShowInput = true;
validation.ShowError = true;
validation.IgnoreBlank = true;
validation.InCellDropDown = true;
// Save the workbook
workbook.Save("ValidationExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
