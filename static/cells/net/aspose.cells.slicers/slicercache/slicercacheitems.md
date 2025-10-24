##SlicerCache.SlicerCacheItems
SlicerCache property. Returns a SlicerCacheItem collection that contains the collection of all items in the slicer cache. Readonly
## SlicerCache.SlicerCacheItems property
Returns a SlicerCacheItem collection that contains the collection of all items in the slicer cache. Read-only
```csharp
public SlicerCacheItemCollection SlicerCacheItems { get; }
```
### Examples
```csharp
[C#]
//get SlicerCacheItem collection that contains the collection of all items in the slicer cache.
SlicerCacheItemCollection slicerCacheItems = slicerCache.SlicerCacheItems;
Console.WriteLine(slicerCacheItems.Count);
```
### See Also
* class [SlicerCacheItemCollection](../../slicercacheitemcollection/)
* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
