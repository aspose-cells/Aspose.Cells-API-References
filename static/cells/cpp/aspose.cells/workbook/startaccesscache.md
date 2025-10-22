##Aspose::Cells::Workbook::StartAccessCache method
'Aspose::Cells::Workbook::StartAccessCache method. Starts the session that uses caches to access data in C++.'
## Workbook::StartAccessCache method
Starts the session that uses caches to access data.
```cpp
void Aspose::Cells::Workbook::StartAccessCache(AccessCacheOptions opts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| opts | AccessCacheOptions | options of data access |
## Remarks
If the cache of specified data access requires some data models in worksheet to be "read-only", then corresponding data models in every worksheet in this workbook will be taken as "read-only" and user should not change any of them.
After finishing the access to the data, [CloseAccessCache(AccessCacheOptions)](../closeaccesscache/) should be invoked with same options to clear all caches and recover normal access mode.
## See Also
* Class [Vector](../../vector/)
* Enum [AccessCacheOptions](../../accesscacheoptions/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
