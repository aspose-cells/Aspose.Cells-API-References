##get_cache_folder method
## get_cache_folder() {#}
Gets the folder for temporary files that may be used as data cache.
### Returns
Folder for cache files that has been specified.
If it has not been specified, null will be returned
and system's temporary path will be used when needed.
```python
@staticmethod
def get_cache_folder():
...
```
### Remarks
Cache files are used generally for some features for memory performance consideration,
such as saving large data set to xls file,
or using memory mode with file cache for cells model.
### See Also
* module [`aspose.cells`](../../)
* class [`CellsHelper`](/cells/python-net/aspose.cells/cellshelper)
