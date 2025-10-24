##Aspose::Cells::Worksheet::StartAccessCache method
'Aspose::Cells::Worksheet::StartAccessCache method. Starts the session that uses caches to access the data in this worksheet in C++.'
## Worksheet::StartAccessCache method
Starts the session that uses caches to access the data in this worksheet.
```cpp
void Aspose::Cells::Worksheet::StartAccessCache(AccessCacheOptions opts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| opts | AccessCacheOptions | options of data access |
## Remarks
After finishing the access to the data, [CloseAccessCache(AccessCacheOptions)](../closeaccesscache/) should be invoked with same options to clear all caches and recover normal access mode.
## See Also
* Class [Vector](../../vector/)
* Enum [AccessCacheOptions](../../accesscacheoptions/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
