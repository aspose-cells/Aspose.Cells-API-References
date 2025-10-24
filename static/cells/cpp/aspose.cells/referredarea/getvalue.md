##Aspose::Cells::ReferredArea::GetValue method
'Aspose::Cells::ReferredArea::GetValue method. Gets cell value with given offset from the top-left of this area in C++.'
## ReferredArea::GetValue(int32_t, int32_t) method
Gets cell value with given offset from the top-left of this area.
```cpp
Aspose::Cells::Object Aspose::Cells::ReferredArea::GetValue(int32_t rowOffset, int32_t colOffset)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int32_t | row offset from the start row of this area |
| colOffset | int32_t | column offset from the start row of this area |
## ReturnValue
"#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.
## See Also
* Class [Object](../../object/)
* Class [Vector](../../vector/)
* Class [ReferredArea](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## ReferredArea::GetValue(int32_t, int32_t, bool) method
Gets cell value with given offset from the top-left of this area.
```cpp
Aspose::Cells::Object Aspose::Cells::ReferredArea::GetValue(int32_t rowOffset, int32_t colOffset, bool calculateFormulas)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | int32_t | row offset from the start row of this area |
| colOffset | int32_t | column offset from the start row of this area |
| calculateFormulas | bool | Whether calculate it recursively if the specified reference is formula |
## ReturnValue
"#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.
## See Also
* Class [Object](../../object/)
* Class [Vector](../../vector/)
* Class [ReferredArea](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
