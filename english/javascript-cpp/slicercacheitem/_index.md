---
title: SlicerCacheItem
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represent slicer data source item
type: docs
url: /javascript-cpp/slicercacheitem/
---

## SlicerCacheItem class

Represent slicer data source item

```javascript
class SlicerCacheItem;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [selected](#selected--)| boolean | Specifies whether the [SlicerCacheItem](../slicercacheitem/) is selected or not. |
| [value](#value--)| string | Readonly. Returns the label text for the slicer item. |


### selected {#selected--}

Specifies whether the [SlicerCacheItem](../slicercacheitem/) is selected or not.

```javascript
selected : boolean;
```


**Remarks**

Please use [ Slicer.SelectItems(string[], bool)](../ slicer.selectitems(string[], bool)/) method instead if you want to select item. Because this refresh operation causes poor performance due to full data reload every time selection changes.

### value {#value--}

Readonly. Returns the label text for the slicer item.

```javascript
value : string;
```



