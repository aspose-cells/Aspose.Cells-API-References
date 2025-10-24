##Aspose::Cells::LoadFilter::StartSheet method
'Aspose::Cells::LoadFilter::StartSheet method. Prepares filter options before loading given worksheet. User''s implementation of LoadFilter can change the LoadDataFilterOptions here to denote how to load data for this worksheet in C++.'
## LoadFilter::StartSheet method
Prepares filter options before loading given worksheet. User's implementation of [LoadFilter](../) can change the LoadDataFilterOptions here to denote how to load data for this worksheet.
```cpp
virtual void Aspose::Cells::LoadFilter::StartSheet(Worksheet &sheet)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | Worksheet\& | The worksheet to be loaded. There are only few properties can be used for the given worksheet object here because most data and properties have not been loaded. The available properties are: [Name](../../name/), Index, VisibilityType |
## See Also
* Class [Vector](../../vector/)
* Class [Worksheet](../../worksheet/)
* Class [LoadFilter](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
