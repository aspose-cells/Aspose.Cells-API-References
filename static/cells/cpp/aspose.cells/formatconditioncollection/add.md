##Aspose::Cells::FormatConditionCollection::Add method
'Aspose::Cells::FormatConditionCollection::Add method. Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting in C++.'
## FormatConditionCollection::Add(const CellArea\&, FormatConditionType, OperatorType, const U16String\&, const U16String\&) method
Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting.
```cpp
Vector<int32_t> Aspose::Cells::FormatConditionCollection::Add(const CellArea &cellArea, FormatConditionType type, OperatorType operatorType, const U16String &formula1, const U16String &formula2)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | const CellArea\& | Conditional formatted cell range. |
| type | FormatConditionType | Type of conditional formatting.It could be one of the members of FormatConditionType. |
| operatorType | OperatorType | Comparison operator.It could be one of the members of OperatorType. |
| formula1 | const U16String\& | The value or expression associated with conditional formatting. |
| formula2 | const U16String\& | The value or expression associated with conditional formatting |
## ReturnValue
[0]:Formatting condition object index;[1] Effected cell rang index.
## Remarks
[OperatorType](../../operatortype/) <set cref= "FormatConditionType">
## See Also
* Class [Vector](../../vector/)
* Class [CellArea](../../cellarea/)
* Enum [FormatConditionType](../../formatconditiontype/)
* Enum [OperatorType](../../operatortype/)
* Class [U16String](../../u16string/)
* Class [FormatConditionCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## FormatConditionCollection::Add(const CellArea\&, FormatConditionType, OperatorType, const char16_t*, const char16_t*) method
Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting.
```cpp
Vector<int32_t> Aspose::Cells::FormatConditionCollection::Add(const CellArea &cellArea, FormatConditionType type, OperatorType operatorType, const char16_t *formula1, const char16_t *formula2)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | const CellArea\& | Conditional formatted cell range. |
| type | FormatConditionType | Type of conditional formatting.It could be one of the members of FormatConditionType. |
| operatorType | OperatorType | Comparison operator.It could be one of the members of OperatorType. |
| formula1 | const char16_t* | The value or expression associated with conditional formatting. |
| formula2 | const char16_t* | The value or expression associated with conditional formatting |
## ReturnValue
[0]:Formatting condition object index;[1] Effected cell rang index.
## Remarks
[OperatorType](../../operatortype/) <set cref= "FormatConditionType">
## See Also
* Class [Vector](../../vector/)
* Class [CellArea](../../cellarea/)
* Enum [FormatConditionType](../../formatconditiontype/)
* Enum [OperatorType](../../operatortype/)
* Class [FormatConditionCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
