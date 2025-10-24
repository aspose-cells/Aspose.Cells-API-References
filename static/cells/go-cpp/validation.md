##Validation Class
'Validation class. Encapsulates the object that represents validation in Go.'
## Validation class
Represents data validation.settings.
```go
type Validation struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetOperator](./getoperator/) | Represents the operator for the data validation. |
|[SetOperator](./setoperator/) | Represents the operator for the data validation. |
|[GetAlertStyle](./getalertstyle/) | Represents the validation alert style. |
|[SetAlertStyle](./setalertstyle/) | Represents the validation alert style. |
|[GetType](./gettype/) | Represents the data validation type. |
|[SetType](./settype/) | Represents the data validation type. |
|[GetInputMessage](./getinputmessage/) | Represents the data validation input message. |
|[SetInputMessage](./setinputmessage/) | Represents the data validation input message. |
|[GetInputTitle](./getinputtitle/) | Represents the title of the data-validation input dialog box. |
|[SetInputTitle](./setinputtitle/) | Represents the title of the data-validation input dialog box. |
|[GetErrorMessage](./geterrormessage/) | Represents the data validation error message. |
|[SetErrorMessage](./seterrormessage/) | Represents the data validation error message. |
|[GetErrorTitle](./geterrortitle/) | Represents the title of the data-validation error dialog box. |
|[SetErrorTitle](./seterrortitle/) | Represents the title of the data-validation error dialog box. |
|[GetShowInput](./getshowinput/) | Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range. |
|[SetShowInput](./setshowinput/) | Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range. |
|[GetShowError](./getshowerror/) | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
|[SetShowError](./setshowerror/) | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
|[GetIgnoreBlank](./getignoreblank/) | Indicates whether blank values are permitted by the range data validation. |
|[SetIgnoreBlank](./setignoreblank/) | Indicates whether blank values are permitted by the range data validation. |
|[GetFormula1_Bool_Bool](./getformula1_bool_bool/) | Gets the value or expression associated with this validation. |
|[GetFormula2_Bool_Bool](./getformula2_bool_bool/) | Gets the value or expression associated with this validation. |
|[GetFormula1_Bool_Bool_Int_Int](./getformula1_bool_bool_int_int/) | Gets the value or expression associated with this validation for specific cell. |
|[GetFormula2_Bool_Bool_Int_Int](./getformula2_bool_bool_int_int/) | Gets the value or expression associated with this validation for specific cell. |
|[SetFormula1_String_Bool_Bool](./setformula1_string_bool_bool/) | Sets the value or expression associated with this validation. |
|[SetFormula2_String_Bool_Bool](./setformula2_string_bool_bool/) | Sets the value or expression associated with this validation. |
|[GetFormula1](./getformula1/) | Represents the value or expression associated with the data validation. |
|[SetFormula1_String](./setformula1_string/) | Represents the value or expression associated with the data validation. |
|[GetFormula2](./getformula2/) | Represents the value or expression associated with the data validation. |
|[SetFormula2_String](./setformula2_string/) | Represents the value or expression associated with the data validation. |
|[GetListValue](./getlistvalue/) | Get the value for list of the validation for the specified cell. |
|[GetValue1](./getvalue1/) | Represents the first value associated with the data validation. |
|[SetValue1](./setvalue1/) | Represents the first value associated with the data validation. |
|[GetValue2](./getvalue2/) | Represents the second value associated with the data validation. |
|[SetValue2](./setvalue2/) | Represents the second value associated with the data validation. |
|[GetValue](./getvalue/) | Get the value of validation on the specific cell. |
|[GetInCellDropDown](./getincelldropdown/) | Indicates whether data validation displays a drop-down list that contains acceptable values. |
|[SetInCellDropDown](./setincelldropdown/) | Indicates whether data validation displays a drop-down list that contains acceptable values. |
|[GetAreas](./getareas/) | Gets all CellArea which contain the data validation settings. |
|[AddArea_CellArea](./addarea_cellarea/) | Applies the validation to the area. |
|[AddArea_CellArea_Bool_Bool](./addarea_cellarea_bool_bool/) | Applies the validation to the area. |
|[AddAreas](./addareas/) | Applies the validation to given areas. |
|[RemoveArea](./removearea/) | Remove the validation settings in the range. |
|[RemoveAreas](./removeareas/) | Removes this validation from given areas. |
|[RemoveACell](./removeacell/) | Remove the validation settings in the cell. |
|[Copy](./copy/) | Copy validation. |
