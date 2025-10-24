##Aspose::Cells::Validation class
'Aspose::Cells::Validation class. Represents data validation.settings in C++.'
## Validation class
Represents data validation.settings.
```cpp
class Validation
```
## Methods
| Method | Description |
| --- | --- |
| [AddArea(const CellArea\& cellArea)](./addarea/) | Applies the validation to the area. |
| [AddArea(const CellArea\& cellArea, bool checkIntersection, bool checkEdge)](./addarea/) | Applies the validation to the area. |
| [AddAreas(const Vector \<CellArea\>\& areas, bool checkIntersection, bool checkEdge)](./addareas/) | Applies the validation to given areas. |
| [Copy(const Validation\& source, const CopyOptions\& copyOption)](./copy/) | Copy validation. |
| [GetAlertStyle()](./getalertstyle/) | Represents the validation alert style. |
| [GetAreas()](./getareas/) | Gets all [CellArea](../cellarea/) which contain the data validation settings. |
| [GetErrorMessage()](./geterrormessage/) | Represents the data validation error message. |
| [GetErrorTitle()](./geterrortitle/) | Represents the title of the data-validation error dialog box. |
| [GetFormula1(bool isR1C1, bool isLocal)](./getformula1/) | Gets the value or expression associated with this validation. |
| [GetFormula1(bool isR1C1, bool isLocal, int32_t row, int32_t column)](./getformula1/) | Gets the value or expression associated with this validation for specific cell. |
| [GetFormula1()](./getformula1/) | Represents the value or expression associated with the data validation. |
| [GetFormula2(bool isR1C1, bool isLocal)](./getformula2/) | Gets the value or expression associated with this validation. |
| [GetFormula2(bool isR1C1, bool isLocal, int32_t row, int32_t column)](./getformula2/) | Gets the value or expression associated with this validation for specific cell. |
| [GetFormula2()](./getformula2/) | Represents the value or expression associated with the data validation. |
| [GetIgnoreBlank()](./getignoreblank/) | Indicates whether blank values are permitted by the range data validation. |
| [GetInCellDropDown()](./getincelldropdown/) | Indicates whether data validation displays a drop-down list that contains acceptable values. |
| [GetInputMessage()](./getinputmessage/) | Represents the data validation input message. |
| [GetInputTitle()](./getinputtitle/) | Represents the title of the data-validation input dialog box. |
| [GetListValue(int32_t row, int32_t column)](./getlistvalue/) | Get the value for list of the validation for the specified cell. |
| [GetOperator()](./getoperator/) | Represents the operator for the data validation. |
| [GetShowError()](./getshowerror/) | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [GetShowInput()](./getshowinput/) | Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range. |
| [GetType()](./gettype/) | Represents the data validation type. |
| [GetValue(int32_t row, int32_t column, bool isValue1)](./getvalue/) | Get the value of validation on the specific cell. |
| [GetValue1()](./getvalue1/) | Represents the first value associated with the data validation. |
| [GetValue2()](./getvalue2/) | Represents the second value associated with the data validation. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Validation\& src)](./operator_asm/) | operator= |
| [RemoveACell(int32_t row, int32_t column)](./removeacell/) | Remove the validation settings in the cell. |
| [RemoveArea(const CellArea\& cellArea)](./removearea/) | Remove the validation settings in the range. |
| [RemoveAreas(const Vector \<CellArea\>\& areas)](./removeareas/) | Removes this validation from given areas. |
| [SetAlertStyle(ValidationAlertType value)](./setalertstyle/) | Represents the validation alert style. |
| [SetErrorMessage(const U16String\& value)](./seterrormessage/) | Represents the data validation error message. |
| [SetErrorMessage(const char16_t* value)](./seterrormessage/) | Represents the data validation error message. |
| [SetErrorTitle(const U16String\& value)](./seterrortitle/) | Represents the title of the data-validation error dialog box. |
| [SetErrorTitle(const char16_t* value)](./seterrortitle/) | Represents the title of the data-validation error dialog box. |
| [SetFormula1(const U16String\& formula, bool isR1C1, bool isLocal)](./setformula1/) | Sets the value or expression associated with this validation. |
| [SetFormula1(const char16_t* formula, bool isR1C1, bool isLocal)](./setformula1/) | Sets the value or expression associated with this validation. |
| [SetFormula1(const U16String\& value)](./setformula1/) | Represents the value or expression associated with the data validation. |
| [SetFormula1(const char16_t* value)](./setformula1/) | Represents the value or expression associated with the data validation. |
| [SetFormula2(const U16String\& formula, bool isR1C1, bool isLocal)](./setformula2/) | Sets the value or expression associated with this validation. |
| [SetFormula2(const char16_t* formula, bool isR1C1, bool isLocal)](./setformula2/) | Sets the value or expression associated with this validation. |
| [SetFormula2(const U16String\& value)](./setformula2/) | Represents the value or expression associated with the data validation. |
| [SetFormula2(const char16_t* value)](./setformula2/) | Represents the value or expression associated with the data validation. |
| [SetIgnoreBlank(bool value)](./setignoreblank/) | Indicates whether blank values are permitted by the range data validation. |
| [SetInCellDropDown(bool value)](./setincelldropdown/) | Indicates whether data validation displays a drop-down list that contains acceptable values. |
| [SetInputMessage(const U16String\& value)](./setinputmessage/) | Represents the data validation input message. |
| [SetInputMessage(const char16_t* value)](./setinputmessage/) | Represents the data validation input message. |
| [SetInputTitle(const U16String\& value)](./setinputtitle/) | Represents the title of the data-validation input dialog box. |
| [SetInputTitle(const char16_t* value)](./setinputtitle/) | Represents the title of the data-validation input dialog box. |
| [SetOperator(OperatorType value)](./setoperator/) | Represents the operator for the data validation. |
| [SetShowError(bool value)](./setshowerror/) | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [SetShowInput(bool value)](./setshowinput/) | Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range. |
| [SetType(ValidationType value)](./settype/) | Represents the data validation type. |
| [SetValue1(const Aspose::Cells::Object\& value)](./setvalue1/) | Represents the first value associated with the data validation. |
| [SetValue2(const Aspose::Cells::Object\& value)](./setvalue2/) | Represents the second value associated with the data validation. |
| [Validation(Validation_Impl* impl)](./validation/) | Constructs from an implementation object. |
| [Validation(const Validation\& src)](./validation/) | Copy constructor. |
| [~Validation()](./~validation/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
ValidationCollection validations = workbook.GetWorksheets().Get(0).GetValidations();
CellArea area = CellArea::CreateCellArea(0, 0, 1, 1);
Validation validation = validations.Get(validations.Add(area));
validation.SetType(ValidationType::WholeNumber);
validation.SetOperator(OperatorType::Between);
validation.SetFormula1(u"3");
validation.SetFormula2(u"1234");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
