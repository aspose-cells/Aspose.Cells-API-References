---
title: Top10Filter
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the top N percent or number of items to filter by.
type: docs
url: /javascript-cpp/top10filter/
---

## Top10Filter class

Represents the top N (percent or number of items) to filter by.

```javascript
class Top10Filter;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(VObject)](#constructor-vobject-)| Constructs from a VObject convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [isTop](#isTop--)| boolean | Indicates whether or not to filter by top order |
| [isPercent](#isPercent--)| boolean | Indicates whether or not to filter by percent value of the column |
| [items](#items--)| number | Gets and sets top or bottom value to use as the filter criteria. |
| [criteria](#criteria--)| VObject | The actual cell value in the range which is used to perform the comparison for this filter. This is the cache value during the refresh process. |

## Methods

| Method | Description |
| --- | --- |
| [toVObject()](#toVObject--)| Gets the VObject. |


### constructor(VObject) {#constructor-vobject-}

Constructs from a VObject convertible to this.

```javascript
constructor(vobj: VObject);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vobj | VObject | The vobject. |

### isTop {#isTop--}

Indicates whether or not to filter by top order

```javascript
isTop : boolean;
```


### isPercent {#isPercent--}

Indicates whether or not to filter by percent value of the column

```javascript
isPercent : boolean;
```


### items {#items--}

Gets and sets top or bottom value to use as the filter criteria.

```javascript
items : number;
```


### criteria {#criteria--}

The actual cell value in the range which is used to perform the comparison for this filter. This is the cache value during the refresh process.

```javascript
criteria : VObject;
```


**Remarks**

NOTE: This member is now obsolete. Instead,please ignore this property. This property will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

### toVObject() {#toVObject--}

Gets the VObject.

```javascript
toVObject() : VObject;
```



