---
title: SlicerCache
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represent summary description of slicer cache
type: docs
url: /nodejs-cpp/slicercache/
---

## SlicerCache class

Represent summary description of slicer cache

```javascript
class SlicerCache;
```


## Methods

| Method | Description |
| --- | --- |
| [getCrossFilterType()](#getCrossFilterType--)| Returns or sets whether a slicer is participating in cross filtering with other slicers that share the same slicer cache, and how cross filtering is displayed. Read/write |
| [setCrossFilterType(SlicerCacheCrossFilterType)](#setCrossFilterType-slicercachecrossfiltertype-)| Returns or sets whether a slicer is participating in cross filtering with other slicers that share the same slicer cache, and how cross filtering is displayed. Read/write |
| [getList()](#getList--)| Returns whether the slicer associated with the specified slicer cache is based on an Non-OLAP data source. Read-only |
| [getSlicerCacheItems()](#getSlicerCacheItems--)| Returns a SlicerCacheItem collection that contains the collection of all items in the slicer cache. Read-only |
| [getName()](#getName--)| Returns the name of the slicer cache. |
| [getSourceName()](#getSourceName--)| Returns the name of this slicer cache. |


### getCrossFilterType() {#getCrossFilterType--}

Returns or sets whether a slicer is participating in cross filtering with other slicers that share the same slicer cache, and how cross filtering is displayed. Read/write

```javascript
getCrossFilterType() : SlicerCacheCrossFilterType;
```


**Returns**

[SlicerCacheCrossFilterType](/nodejs-cpp/slicercachecrossfiltertype/)

### setCrossFilterType(SlicerCacheCrossFilterType) {#setCrossFilterType-slicercachecrossfiltertype-}

Returns or sets whether a slicer is participating in cross filtering with other slicers that share the same slicer cache, and how cross filtering is displayed. Read/write

```javascript
setCrossFilterType(value: SlicerCacheCrossFilterType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SlicerCacheCrossFilterType](/nodejs-cpp/slicercachecrossfiltertype/) | The value to set. |

### getList() {#getList--}

Returns whether the slicer associated with the specified slicer cache is based on an Non-OLAP data source. Read-only

```javascript
getList() : boolean;
```


### getSlicerCacheItems() {#getSlicerCacheItems--}

Returns a SlicerCacheItem collection that contains the collection of all items in the slicer cache. Read-only

```javascript
getSlicerCacheItems() : SlicerCacheItemCollection;
```


**Returns**

[SlicerCacheItemCollection](/nodejs-cpp/slicercacheitemcollection/)

### getName() {#getName--}

Returns the name of the slicer cache.

```javascript
getName() : string;
```


### getSourceName() {#getSourceName--}

Returns the name of this slicer cache.

```javascript
getSourceName() : string;
```



