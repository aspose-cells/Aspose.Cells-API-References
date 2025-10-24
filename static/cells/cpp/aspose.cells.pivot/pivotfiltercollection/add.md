##Aspose::Cells::Pivot::PivotFilterCollection::Add method
'Aspose::Cells::Pivot::PivotFilterCollection::Add method. Adds a PivotFilterObject to the specific type in C++.'
## PivotFilterCollection::Add method
Adds a [PivotFilter](../../pivotfilter/)[Object](../../../aspose.cells/object/) to the specific type.
>Deprecated
>
>Use PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() and AddDateFilter() methods,instead.
```cpp
int32_t Aspose::Cells::Pivot::PivotFilterCollection::Add(int32_t fieldIndex, PivotFilterType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int32_t | the [PivotField](../../pivotfield/) index |
| type | PivotFilterType | the [PivotFilter](../../pivotfilter/) type |
## ReturnValue
the index of the [PivotFilter](../../pivotfilter/)[Object](../../../aspose.cells/object/) in this [PivotFilterCollection](../).
## Remarks
NOTE: This method is now obsolete. Instead, please use [PivotFilterCollection.AddValueFilter()](../addvaluefilter/),[AddTop10Filter()](../addtop10filter/),[AddLabelFilter()](../addlabelfilter/) and [AddDateFilter()](../adddatefilter/) methods. This method will be removed 12 months later since November 2024. **Aspose** apologizes for any inconvenience you may have experienced.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Enum [PivotFilterType](../../pivotfiltertype/)
* Class [PivotFilterCollection](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
