##Aspose::Cells::LightCellsDataProvider::IsGatherString method
'Aspose::Cells::LightCellsDataProvider::IsGatherString method. Checks whether the current string value of cell needs to be gathered into a global pool in C++.'
## LightCellsDataProvider::IsGatherString method
Checks whether the current string value of cell needs to be gathered into a global pool.
```cpp
virtual bool Aspose::Cells::LightCellsDataProvider::IsGatherString()=0
```
## ReturnValue
true if string value need to be gathered into a global pool for the resultant file.
## Remarks
Gathering string values will take advantage only when there are many duplicated string values for the cells provided by this implementation. In this situation gathering string will save much memory and generate smaller resultant file. If there are many string values for the cells provided by [LightCellsDataProvider](../) but few of them are same, gathering string will cost more memory and time and has no advantage for the resultant file.
## See Also
* Class [Vector](../../vector/)
* Class [LightCellsDataProvider](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
