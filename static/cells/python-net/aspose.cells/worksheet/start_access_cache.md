##start_access_cache method
## start_access_cache(self, opts) {#aspose.cells.AccessCacheOptions}
Starts the session that uses caches to access the data in this worksheet.
```python
def start_access_cache(self, opts):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| opts | aspose.cells.AccessCacheOptions | options of data access |
### Remarks
After finishing the access to the data, [`Worksheet.close_access_cache`](/cells/python-net/aspose.cells/worksheet/close_access_cache) should
be invoked with same options to clear all caches and recover normal access mode.
### See Also
* module [`aspose.cells`](../../)
* class [`Worksheet`](/cells/python-net/aspose.cells/worksheet)
