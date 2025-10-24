##start_access_cache method
## start_access_cache(self, opts) {#aspose.cells.AccessCacheOptions}
Starts the session that uses caches to access data.
```python
def start_access_cache(self, opts):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| opts | aspose.cells.AccessCacheOptions | options of data access |
### Remarks
If the cache of specified data access requires some data models in worksheet to be "read-only",
then corresponding data models in every worksheet in this workbook will be taken as "read-only"
and user should not change any of them.
After finishing the access to the data, [`Workbook.close_access_cache`](/cells/python-net/aspose.cells/workbook/close_access_cache) should
be invoked with same options to clear all caches and recover normal access mode.
### See Also
* module [`aspose.cells`](../../)
* class [`Workbook`](/cells/python-net/aspose.cells/workbook)
