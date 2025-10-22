##Aspose::Cells::WorksheetCollection::RegisterAddInFunction method
'Aspose::Cells::WorksheetCollection::RegisterAddInFunction method. Adds addin function into the workbook in C++.'
## WorksheetCollection::RegisterAddInFunction(const U16String\&, const U16String\&, bool) method
Adds addin function into the workbook.
```cpp
int32_t Aspose::Cells::WorksheetCollection::RegisterAddInFunction(const U16String &addInFile, const U16String &functionName, bool lib)
```
| Parameter | Type | Description |
| --- | --- | --- |
| addInFile | const U16String\& | the file contains the addin functions |
| functionName | const U16String\& | the addin function name |
| lib | bool | whether the given addin file is in the directory or sub-directory of [Workbook](../../workbook/) Add-In library. This flag takes effect and makes difference when given addInFile is of relative path: true denotes the path is relative to Add-In library and false denotes the path is relative to this [Workbook](../../workbook/). |
## ReturnValue
ID of the data which contains given addin function
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [WorksheetCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## WorksheetCollection::RegisterAddInFunction(const char16_t*, const char16_t*, bool) method
Adds addin function into the workbook.
```cpp
int32_t Aspose::Cells::WorksheetCollection::RegisterAddInFunction(const char16_t *addInFile, const char16_t *functionName, bool lib)
```
| Parameter | Type | Description |
| --- | --- | --- |
| addInFile | const char16_t* | the file contains the addin functions |
| functionName | const char16_t* | the addin function name |
| lib | bool | whether the given addin file is in the directory or sub-directory of [Workbook](../../workbook/) Add-In library. This flag takes effect and makes difference when given addInFile is of relative path: true denotes the path is relative to Add-In library and false denotes the path is relative to this [Workbook](../../workbook/). |
## ReturnValue
ID of the data which contains given addin function
## See Also
* Class [Vector](../../vector/)
* Class [WorksheetCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## WorksheetCollection::RegisterAddInFunction(int32_t, const U16String\&) method
Adds addin function into the workbook.
```cpp
U16String Aspose::Cells::WorksheetCollection::RegisterAddInFunction(int32_t id, const U16String &functionName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| id | int32_t | ID of the data which contains addin functions, can be got by the first call of RegisterAddInFunction(string, string, bool) for the same addin file. |
| functionName | const U16String\& | the addin function name |
## ReturnValue
URL of the addin file which contains addin functions
## See Also
* Class [U16String](../../u16string/)
* Class [Vector](../../vector/)
* Class [WorksheetCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## WorksheetCollection::RegisterAddInFunction(int32_t, const char16_t*) method
Adds addin function into the workbook.
```cpp
U16String Aspose::Cells::WorksheetCollection::RegisterAddInFunction(int32_t id, const char16_t *functionName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| id | int32_t | ID of the data which contains addin functions, can be got by the first call of RegisterAddInFunction(string, string, bool) for the same addin file. |
| functionName | const char16_t* | the addin function name |
## ReturnValue
URL of the addin file which contains addin functions
## See Also
* Class [U16String](../../u16string/)
* Class [Vector](../../vector/)
* Class [WorksheetCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
