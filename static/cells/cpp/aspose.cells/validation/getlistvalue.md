##Aspose::Cells::Validation::GetListValue method
'Aspose::Cells::Validation::GetListValue method. Get the value for list of the validation for the specified cell in C++.'
## Validation::GetListValue method
Get the value for list of the validation for the specified cell.
```cpp
Aspose::Cells::Object Aspose::Cells::Validation::GetListValue(int32_t row, int32_t column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | int32_t | The row index. |
| column | int32_t | The column index. |
## ReturnValue
The value to produce the list of this validation for the specified cell. If the list references to a range, then the returned value will be a [ReferredArea](../../referredarea/) object; Otherwise the returned value may be null, object[], or simple object.
## Remarks
Only for validation whose type is List and has been applied to given cell, otherwise null will be returned.
## See Also
* Class [Object](../../object/)
* Class [Vector](../../vector/)
* Class [Validation](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
