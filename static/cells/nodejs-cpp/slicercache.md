##SlicerCache
Represent summary description of slicer cache
## SlicerCache class
Represent summary description of slicer cache
```javascript
class SlicerCache;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [crossFilterType](#crossFilterType--)| SlicerCacheCrossFilterType | Returns or sets whether a slicer is participating in cross filtering with other slicers that share the same slicer cache, and how cross filtering is displayed. Read/write |
| [list](#list--)| boolean | Readonly. Returns whether the slicer associated with the specified slicer cache is based on an Non-OLAP data source. Read-only |
| [slicerCacheItems](#slicerCacheItems--)| SlicerCacheItemCollection | Readonly. Returns a SlicerCacheItem collection that contains the collection of all items in the slicer cache. Read-only |
| [name](#name--)| string | Readonly. Returns the name of the slicer cache. |
| [sourceName](#sourceName--)| string | Readonly. Returns the name of this slicer cache. |
## Methods
| Method | Description |
| --- | --- |
| [getCrossFilterType()](#getCrossFilterType--)| <b>@deprecated.</b> Please use the 'crossFilterType' property instead. Returns or sets whether a slicer is participating in cross filtering with other slicers that share the same slicer cache, and how cross filtering is displayed. Read/write |
| [setCrossFilterType(SlicerCacheCrossFilterType)](#setCrossFilterType-slicercachecrossfiltertype-)| <b>@deprecated.</b> Please use the 'crossFilterType' property instead. Returns or sets whether a slicer is participating in cross filtering with other slicers that share the same slicer cache, and how cross filtering is displayed. Read/write |
| [getList()](#getList--)| <b>@deprecated.</b> Please use the 'list' property instead. Returns whether the slicer associated with the specified slicer cache is based on an Non-OLAP data source. Read-only |
| [getSlicerCacheItems()](#getSlicerCacheItems--)| <b>@deprecated.</b> Please use the 'slicerCacheItems' property instead. Returns a SlicerCacheItem collection that contains the collection of all items in the slicer cache. Read-only |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Returns the name of the slicer cache. |
| [getSourceName()](#getSourceName--)| <b>@deprecated.</b> Please use the 'sourceName' property instead. Returns the name of this slicer cache. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### crossFilterType {#crossFilterType--}
Returns or sets whether a slicer is participating in cross filtering with other slicers that share the same slicer cache, and how cross filtering is displayed. Read/write
```javascript
crossFilterType : SlicerCacheCrossFilterType;
```
### list {#list--}
Readonly. Returns whether the slicer associated with the specified slicer cache is based on an Non-OLAP data source. Read-only
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
### getCrossFilterType() {#getCrossFilterType--}
```javascript
getCrossFilterType() : SlicerCacheCrossFilterType;
```
**Returns**
[SlicerCacheCrossFilterType](../slicercachecrossfiltertype/)
### setCrossFilterType(SlicerCacheCrossFilterType) {#setCrossFilterType-slicercachecrossfiltertype-}
```javascript
setCrossFilterType(value: SlicerCacheCrossFilterType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SlicerCacheCrossFilterType](../slicercachecrossfiltertype/) | The value to set. |
### getList() {#getList--}
```javascript
getList() : boolean;
```
### getSlicerCacheItems() {#getSlicerCacheItems--}
```javascript
getSlicerCacheItems() : SlicerCacheItemCollection;
```
**Returns**
[SlicerCacheItemCollection](../slicercacheitemcollection/)
### getName() {#getName--}
```javascript
getName() : string;
```
### getSourceName() {#getSourceName--}
```javascript
getSourceName() : string;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
