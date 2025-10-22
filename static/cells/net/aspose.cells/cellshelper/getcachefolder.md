##CellsHelper.GetCacheFolder
CellsHelper method. Gets the folder for temporary files that may be used as data cache
## CellsHelper.GetCacheFolder method
Gets the folder for temporary files that may be used as data cache.
```csharp
public static string GetCacheFolder()
```
### Return Value
Folder for cache files that has been specified. If it has not been specified, null will be returned and system's temporary path will be used when needed.
### Remarks
Cache files are used generally for some features for memory performance consideration, such as saving large data set to xls file, or using memory mode with file cache for cells model.
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
