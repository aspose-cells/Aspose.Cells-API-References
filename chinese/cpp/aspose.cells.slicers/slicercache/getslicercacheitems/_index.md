---
title: Aspose::Cells::Slicers::SlicerCache::GetSlicerCacheItems method
linktitle: GetSlicerCacheItems
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Slicers::SlicerCache::GetSlicerCacheItems method. Returns a SlicerCacheItem collection that contains the collection of all items in the slicer cache. Read-only in C++.'
type: docs
weight: 900
url: /zh/cpp/aspose.cells.slicers/slicercache/getslicercacheitems/
---
## SlicerCache::GetSlicerCacheItems method


Returns a [SlicerCacheItem](../../slicercacheitem/) collection that contains the collection of all items in the slicer cache. Read-only.

```cpp
SlicerCacheItemCollection Aspose::Cells::Slicers::SlicerCache::GetSlicerCacheItems()
```


## Examples


```cpp
//获取 SlicerCacheItem 集合，该集合包含切片器缓存中所有项目的集合。
SlicerCacheItemCollection slicerCacheItems = slicerCache.GetSlicerCacheItems();
std::cout << slicerCacheItems.GetCount() <<std::endl;
```

## See Also

* Class [SlicerCacheItemCollection](../../slicercacheitemcollection/)
* Class [SlicerCache](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
