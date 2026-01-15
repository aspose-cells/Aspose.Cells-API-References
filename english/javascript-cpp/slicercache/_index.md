---
title: SlicerCache
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represent summary description of slicer cache
type: docs
url: /javascript-cpp/slicercache/
---

## SlicerCache class

Represent summary description of slicer cache

```javascript
class SlicerCache;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [crossFilterType](#crossFilterType--)| SlicerCacheCrossFilterType | Indicates how to show items with no data of slicer. |
| [list](#list--)| boolean | Readonly. Indicates whether the slicer associated with the specified slicer cache is based on an Non-OLAP data source. |
| [slicerCacheItems](#slicerCacheItems--)| SlicerCacheItemCollection | Readonly. Returns a SlicerCacheItem collection that contains the collection of all items in the slicer cache. Read-only |
| [name](#name--)| string | Readonly. Returns the name of the slicer cache. |
| [sourceName](#sourceName--)| string | Readonly. Returns the name of this slicer cache. |


### crossFilterType {#crossFilterType--}

Indicates how to show items with no data of slicer.

```javascript
crossFilterType : SlicerCacheCrossFilterType;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [Slicer.ShowTypeOfItemsWithNoData](../slicer.showtypeofitemswithnodata/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### list {#list--}

Readonly. Indicates whether the slicer associated with the specified slicer cache is based on an Non-OLAP data source.

```javascript
list : boolean;
```


### slicerCacheItems {#slicerCacheItems--}

Readonly. Returns a SlicerCacheItem collection that contains the collection of all items in the slicer cache. Read-only

```javascript
slicerCacheItems : SlicerCacheItemCollection;
```


### name {#name--}

Readonly. Returns the name of the slicer cache.

```javascript
name : string;
```


### sourceName {#sourceName--}

Readonly. Returns the name of this slicer cache.

```javascript
sourceName : string;
```



